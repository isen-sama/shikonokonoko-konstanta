# shikonokonoko-konstanta

โปรเจกต์นี้ประกอบด้วยสคริปต์ Python และไฟล์สเปคสำหรับการ build ด้วย PyInstaller

## โครงสร้างโปรเจกต์

```
shikonokonoko-konstanta/
├── README.md
├── test.py
├── test.spec
└── build/
    └── test/
        ├── Analysis-00.toc
        ├── base_library.zip
        ├── EXE-00.toc
        ├── PKG-00.toc
        ├── PYZ-00.pyz
        ├── PYZ-00.toc
        ├── test.pkg
        ├── warn-test.txt
        ├── xref-test.html
        └── localpycs/
            ├── pyimod01_archive.pyc
            ├── pyimod02_importers.pyc
            ├── pyimod03_ctypes.pyc
            ├── pyimod04_pywin32.pyc
            └── struct.pyc
```

## วิธีการ build

1. ติดตั้ง [PyInstaller](https://pyinstaller.org/)
2. ใช้คำสั่งนี้เพื่อ build ไฟล์ `test.py`:
    ```sh
    pyinstaller test.spec
    ```
3. ไฟล์ที่ build แล้วจะอยู่ในโฟลเดอร์ `build/test/`

## ไฟล์สำคัญ

- [test.py](shikonokonoko-konstanta/test.py) — สคริปต์ Python หลัก
- [test.spec](shikonokonoko-konstanta/test.spec) — ไฟล์สเปคสำหรับ PyInstaller

## หมายเหตุ

- โฟลเดอร์ `build/` จะถูกสร้างขึ้นโดยอัตโนมัติหลังจาก build
- เหมาะสำหรับการทดลองและศึกษาการใช้งาน PyInstaller

---
