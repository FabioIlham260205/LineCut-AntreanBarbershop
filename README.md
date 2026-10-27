# LineCut-AntreanBarbershop


# Struktur Folder Project LineCut

```text
LineCut/
├── frontend/                         # Fabio + Tio
│   ├── package.json                  # Konfigurasi frontend
│   ├── public/                       # Fabio
│   │   ├── manifest.json             # Konfigurasi PWA
│   │   └── icons/                    # Ikon aplikasi
│   └── src/
│       ├── components/               # Fabio + Tio
│       ├── pages/
│       │   ├── customer/             # Fabio
│       │   │   ├── BookingPage.jsx
│       │   │   ├── BookingDetail.jsx
│       │   │   └── QueuePage.jsx
│       │   ├── admin/                # Tio
│       │   │   ├── DashboardPage.jsx
│       │   │   ├── QueueManagement.jsx
│       │   │   ├── ReportsPage.jsx
│       │   │   └── SettingsPage.jsx
│       │   └── barber/               # Tio
│       │       └── BarberQueue.jsx
│       ├── services/                 # Fabio + Tio
│       │   └── api.js                # Penghubung frontend ke backend
│       ├── App.jsx                   # Fabio
│       └── main.jsx                  # Fabio
│
├── backend/                          # Bagas
│   ├── package.json                  # Konfigurasi backend
│   ├── app/
│   │   └── api/
│   │       ├── bookings/             # API pemesanan
│   │       ├── queue/                # API antrean
│   │       ├── notifications/        # API notifikasi
│   │       └── auth/                 # API login staf
│   ├── lib/
│   │   └── db.js                     # Koneksi database Neon
│   └── .env.example                  # Contoh konfigurasi environment
│
├── database/                         # Bagas
│   └── schema.sql                    # Struktur tabel database
│
├── docs/                             # Semua anggota
│   ├── ui-ux/                        # Fabio
│   ├── api/                          # Bagas
│   └── testing/                      # Semua anggota
│
├── README.md                         # Dokumentasi project
└── .gitignore                        # Bagas
```

## Pembagian Tanggung Jawab

| Anggota | Bagian yang Dikerjakan |
|---|---|
| Fabio Ilham Muhammad | Halaman customer, booking, informasi antrean, pembatalan antrean, dan UI/UX customer. |
| Bagas Eka Putra | Backend API, sistem antrean, pengelolaan status antrean, database Neon PostgreSQL, dan dokumentasi API. |
| Mochamad Tio Saputra | Halaman admin dan barber, login staf, dashboard, laporan, pengaturan, dan UI notifikasi. |
| Semua anggota | Integrasi sistem, pengujian aplikasi, dokumentasi, dan README. |

## Teknologi yang Digunakan

- **Frontend:** React.js
- **Backend:** Next.js
- **Database:** Neon PostgreSQL
- **Platform:** Progressive Web App (PWA)

## Keterangan

- Customer dapat melakukan pemesanan, melihat nomor dan posisi antrean, memperkirakan waktu tunggu, serta membatalkan antrean selama statusnya masih `WAITING`.
- Admin mengelola antrean, dashboard, laporan, dan pengaturan.
- Barber memperbarui status pelayanan dan memanggil pelanggan berikutnya.
- Notifikasi digunakan untuk memberikan informasi perkembangan antrean kepada pelanggan.
- Project ini ditujukan untuk satu cabang barbershop dan satu jenis layanan, yaitu potong rambut.
```
