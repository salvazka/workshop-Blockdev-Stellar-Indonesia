<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/564a21c8-af2b-44ca-8fad-1df4de86bee3" /># workshop-Blockdev-Stellar-Indonesia
workshop at Stellar Indonesia
Stellar Crowdfunding Workshop
Proyek full-stack DApp untuk membangun platform crowdfunding terdesentralisasi di blockchain Stellar. Menggabungkan frontend React modern dengan backend kontrak pintar Rust/Soroban. Dirancang untuk tujuan edukasi di Stellar Indonesia Workshop (Oktober 2025).

📂 Struktur Proyek
crowdfunding/   # Frontend (React + TypeScript, Vite, TailwindCSS)
ezcrow/         # Kontrak Pintar (Rust + Soroban untuk Stellar)
💻 Frontend (crowdfunding/)
Antarmuka pengguna DApp, dibangun dengan:

React, TypeScript, Vite, dan TailwindCSS.

Menggunakan React Router untuk navigasi.

Terintegrasi dengan dompet dan SDK Stellar.

Mendukung HMR (Hot Module Replacement) untuk pengembangan cepat.

Quick Start
Masuk ke direktori frontend:

Bash

cd crowdfunding
Instal dependensi:

Bash

npm install
Jalankan aplikasi:

Bash

npm run dev
# Kunjungi http://localhost:5173
Build & Deploy
Production build: npm run build

Docker support: docker build -t my-app . && docker run -p 3000:3000 my-app

⚙️ Smart Contracts (ezcrow/)
Logika on-chain inti DApp, ditulis dalam Rust menggunakan Soroban SDK.

Kontrak Utama: contracts/crowdfunding

Fitur: Pembuatan kampanye, donasi, logika target (goal) dan batas waktu (deadline), storage, dan fungsi Refund (pengembalian dana).

Quick Start
Masuk ke direktori kontrak:

Bash

cd ezcrow/contracts/crowdfunding
Build kontrak:

Bash

make build      # Build kontrak
Jalankan unit test:

Bash

make test       # Jalankan tes
# Lihat README.md di folder ini untuk panduan deployment
💡 Konsep Utama
Kampanye memiliki owner, target (goal), dan deadline.

Siapa pun dapat berdonasi; semua logika (termasuk Refund) sepenuhnya on-chain.

Mempelajari dasar Rust, Soroban, dan pengembangan Stellar.

🔗 Resources
Stellar Documentation

Soroban Examples

Risein Platform

BlockDevId Community

Workshop Documentation (Blockdev x Risein x Stellar)
