# Jaring Super Apps - Product Requirements Document (PRD)

**Nama Produk** : Jaring Super Apps (Jaring Hijau Nusantara)  
**Versi**       : 1.0  
**Tanggal**     : 31 Maret 2026  
**Platform**    : Progressive Web App (PWA) – Mobile Web App (Mobile-First)  
**Product Owner**: Amati Indonesia  

## 1. Pendahuluan

### 1.1 Visi
Membangun satu platform super apps yang **sederhana** namun **luar biasa** untuk memberdayakan Petani Mandiri dan komunitas lokal Nusantara dalam mencapai kedaulatan pangan berbasis ekologi.  

Platform ini menyatukan assessment, monitoring real-time, pelaporan, manajemen dana, catatan panen, dan dukungan cerdas dalam satu aplikasi yang ringan dan mudah digunakan.

### 1.2 Tujuan Bisnis
- Mempercepat pemetaan & pendampingan komunitas dari level Basic → Intermediate → Advanced  
- Memberikan transparansi dana, hasil panen, dan kondisi lahan secara real-time  
- Mengurangi kerugian melalui deteksi dini kerusakan lahan  
- Meningkatkan produktivitas kebun pangan dengan data cuaca + harga pasar  
- Memungkinkan petani bekerja tanpa internet (offline wajib)  

### 1.3 Scope Utama (MVP)
Fokus utama: **Kebun Pangan** (dapat dikembangkan ke ternak, ikan, lebah di fase berikutnya).

## 2. Target Pengguna (dari survey PRD)

**Pengguna Utama**  
- **Petani Mandiri** & Ketua Kelompok Tani (usia 35–55 tahun, literasi digital menengah)  

**Pengguna Pendukung**  
- Mentor Wilayah  
- Admin Amati Indonesia  

**Kebutuhan Khusus**  
- Offline mode **wajib**  
- Notifikasi utama via **WhatsApp**  
- Data cuaca krusial: Curah Hujan, Suhu Udara, Kelembaban, Angin  
- Integrasi **harga pasar** komoditas  
- Fokus komoditas: Kebun Pangan  

## 3. Fitur Utama (Simple tapi Luar Biasa)

### 3.1 Assessment & Register
- Form identitas kelompok, lokasi lahan, komoditas, kapasitas, dan sosial  
- Generate token unik  
- Proses review Mentor hingga kategori **Basic / Intermediate / Advanced**  
- Otomatis menentukan rencana lahan & target capaian  

### 3.2 Main Dashboard
- Ringkasan dana (total, terealisasi, sisa)  
- Progress tanaman, jadwal panen & MBG  
- Widget cuaca real-time  
- Quick actions: Catat Panen, Lapor Kerusakan, Minta Dana Cair, Chat Mentor  
- Komentar mentor langsung  

### 3.3 Pusat Pelaporan
- 6 jenis laporan: General, Per Tanaman, Panen, Harian, Mingguan, Bulanan  
- Tracking alokasi dana (Benih, Pupuk, Sarpras, Infrastruktur, Operasional)  
- Riwayat dana cair dengan status Approved/Revisions/Rejected  

### 3.4 Catatan Hasil Panen
- Input komoditas, tanggal panen, berat aktual, kualitas (Grade A/B), foto  
- Monitoring target vs realisasi + jadwal rotasi tanaman  
- Berlaku juga untuk area ternak, ikan, lebah  

### 3.5 Manajemen Kerusakan Lahan
- Laporan kerusakan infrastruktur/alat/bangunan  
- Status tiket + prioritas (Low/Medium/High) + SLA  
- Timeline perbaikan  

### 3.6 AI Assistant & Bantuan
- Chat QnA berbasis AI (cepat & luas) untuk pertanyaan pertanian  
- Pusat Bantuan (FAQ)  
- Direct discussion dengan Mentor/Admin via WhatsApp  

### 3.7 Fitur Pendukung Luar Biasa
- **Offline Mode** (wajib) – isi laporan, catat panen, lapor kerusakan tanpa internet → auto-sync saat online  
- Notifikasi utama **WhatsApp** + push notification cadangan  
- Integrasi data cuaca 4 parameter krusial  
- Integrasi harga pasar komoditas real-time  

## 4. User Journey Utama

1. Login/Register → Assessment → Token & status  
2. Dashboard → Monitoring harian  
3. Catat Panen / Lapor Kerusakan (bisa offline) → Submit → Notif WhatsApp  
4. Review Mentor / AI → Update status  
5. Pusat Pelaporan → Riwayat lengkap  

## 5. Persyaratan Teknis & Non-Functional

- **Teknologi Rekomendasi**  
  - Frontend: Next.js / React + Tailwind (PWA)  
  - Backend: Supabase / Firebase (real-time & offline sync)  
  - Database: PostgreSQL + IndexedDB (offline)  
  - AI: Grok / OpenAI API  
  - Notifikasi: WhatsApp Business API  

- **Offline-First**: Service Worker + IndexedDB  
- **Performance**: Loading < 2 detik, ringan untuk HP low-end  
- **Keamanan**: Role-based access (Petani / Mentor / Admin)  
- **UI/UX**: Tema hijau alam modern-bold, mobile-first, bahasa Indonesia  
- **Accessibility**: WCAG 2.1 AA  

## 6. MVP Scope & Roadmap

**Phase 1 – MVP (3 bulan)**  
- Assessment + Dashboard  
- Pusat Pelaporan + Catatan Hasil Panen  
- Manajemen Kerusakan Lahan  
- Offline Mode + WhatsApp Notif  

**Phase 2 (3 bulan berikutnya)**  
- AI Assistant full  
- Integrasi cuaca + harga pasar  
- Advanced analytics  

## 7. Success Metrics (KPIs)

- 500+ kelompok tani aktif dalam 6 bulan pertama  
- Tingkat penggunaan offline > 40%  
- Akurasi pelaporan panen > 90%  
- Komunitas naik level (Basic → Advanced) > 70% dalam 1 tahun  
- NPS pengguna > 75  

---
# Jaring Super Apps - Product Requirements Document (PRD)

**Nama Produk** : Jaring Super Apps (Jaring Hijau Nusantara)  
**Versi**       : 1.0  
**Tanggal**     : 31 Maret 2026  
**Platform**    : Progressive Web App (PWA) – Mobile Web App (Mobile-First)  
**Product Owner**: Amati Indonesia  

## 1. Pendahuluan

### 1.1 Visi
Membangun satu platform super apps yang **sederhana** namun **luar biasa** untuk memberdayakan Petani Mandiri dan komunitas lokal Nusantara dalam mencapai kedaulatan pangan berbasis ekologi.  
Platform ini menyatukan assessment, monitoring real-time, pelaporan, manajemen dana, catatan panen, dan dukungan cerdas dalam satu aplikasi yang ringan dan mudah digunakan.

### 1.2 Tujuan Bisnis
- Mempercepat pemetaan & pendampingan komunitas dari level Basic → Intermediate → Advanced  
- Memberikan transparansi dana, hasil panen, dan kondisi lahan secara real-time  
- Mengurangi kerugian melalui deteksi dini kerusakan lahan  
- Meningkatkan produktivitas kebun pangan dengan data cuaca + harga pasar  
- Memungkinkan petani bekerja tanpa internet (offline wajib)  

### 1.3 Scope Utama (MVP)
Fokus utama: **Kebun Pangan** (dapat dikembangkan ke ternak, ikan, lebah di fase berikutnya).

## 2. Target Pengguna (dari survey PRD)
**Pengguna Utama**  
- **Petani Mandiri** & Ketua Kelompok Tani (usia 35–55 tahun, literasi digital menengah)  

**Pengguna Pendukung**  
- Mentor Wilayah  
- Admin Amati Indonesia  

**Kebutuhan Khusus**  
- Offline mode **wajib**  
- Notifikasi utama via **WhatsApp**  
- Data cuaca krusial: Curah Hujan, Suhu Udara, Kelembaban, Angin  
- Integrasi **harga pasar** komoditas  
- Fokus komoditas: Kebun Pangan  

## 3. Fitur Utama (Simple tapi Luar Biasa)
### 3.1 Assessment & Register
- Form identitas kelompok, lokasi lahan, komoditas, kapasitas, dan sosial  
- Generate token unik  
- Proses review Mentor hingga kategori **Basic / Intermediate / Advanced**  
- Otomatis menentukan rencana lahan & target capaian  

### 3.2 Main Dashboard
- Ringkasan dana (total, terealisasi, sisa)  
- Progress tanaman, jadwal panen & MBG  
- Widget cuaca real-time  
- Quick actions: Catat Panen, Lapor Kerusakan, Minta Dana Cair, Chat Mentor  
- Komentar mentor langsung  

### 3.3 Pusat Pelaporan
- 6 jenis laporan: General, Per Tanaman, Panen, Harian, Mingguan, Bulanan  
- Tracking alokasi dana (Benih, Pupuk, Sarpras, Infrastruktur, Operasional)  
- Riwayat dana cair dengan status Approved/Revisions/Rejected  

### 3.4 Catatan Hasil Panen
- Input komoditas, tanggal panen, berat aktual, kualitas (Grade A/B), foto  
- Monitoring target vs realisasi + jadwal rotasi tanaman  
- Berlaku juga untuk area ternak, ikan, lebah  

### 3.5 Manajemen Kerusakan Lahan
- Laporan kerusakan infrastruktur/alat/bangunan  
- Status tiket + prioritas (Low/Medium/High) + SLA  
- Timeline perbaikan  

### 3.6 AI Assistant & Bantuan
- Chat QnA berbasis AI (cepat & luas) untuk pertanyaan pertanian  
- Pusat Bantuan (FAQ)  
- Direct discussion dengan Mentor/Admin via WhatsApp  

### 3.7 Fitur Pendukung Luar Biasa
- **Offline Mode** (wajib) – isi laporan, catat panen, lapor kerusakan tanpa internet → auto-sync saat online  
- Notifikasi utama **WhatsApp** + push notification cadangan  
- Integrasi data cuaca 4 parameter krusial  
- Integrasi harga pasar komoditas real-time  

## 4. User Journey Utama
1. Login/Register → Assessment → Token & status  
2. Dashboard → Monitoring harian  
3. Catat Panen / Lapor Kerusakan (bisa offline) → Submit → Notif WhatsApp  
4. Review Mentor / AI → Update status  
5. Pusat Pelaporan → Riwayat lengkap  

## 5. Architecture
```mermaid
graph TD
    A[Petani - HP Android Low-End] --> B[Frontend: Next.js + Tailwind PWA]
    B --> C[Service Worker + IndexedDB Offline]
    C --> D[Supabase Backend Realtime]
    D --> E[(PostgreSQL Database)]
    D --> F[WhatsApp Business API]
    D --> G[AI Assistant Grok/OpenAI]
    H[Mentor/Admin] --> D
