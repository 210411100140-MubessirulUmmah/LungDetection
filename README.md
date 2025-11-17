# Lung CT Scan Detection App (Flask + YOLOv8 + MySQL)

Aplikasi web berbasis **Flask** untuk melakukan **deteksi penyakit paru** dari citra **CT Scan** menggunakan model **YOLOv8**.  
Aplikasi ini mendukung **multi-workspace**, **Google OAuth login**, serta **penyimpanan hasil deteksi** di database MySQL.

---

## 🎬 Demo Aplikasi


https://github.com/user-attachments/assets/d28586a5-c238-464c-addd-706358750f56




## 🚀 Features

### 🔐 User Authentication
- Register & login dengan username/password  
- Login dengan **Google OAuth2**  
- Password aman menggunakan **bcrypt**

---

### 📁 Workspace Management
User dapat:
- Membuat workspace baru
- Melihat semua workspace
- Menyimpan banyak deteksi dalam setiap workspace
- Menghapus workspace beserta seluruh deteksi di dalamnya

---

### 🖼 Image Detection (YOLOv8)
- Upload gambar CT scan paru
- Sistem memproses gambar dengan model `best14.pt`
- Menghasilkan:
  - Bounding box  
  - Class label  
  - Confidence score  
- Menyimpan:
  - Gambar asli  
  - Gambar anotasi  
  - JSON hasil deteksi  

---

### 📦 Download Hasil Deteksi
- Download satu gambar terdeteksi
- Download semua deteksi dalam bentuk ZIP:
  - versi **JSON**
  - versi **Image + TXT**
