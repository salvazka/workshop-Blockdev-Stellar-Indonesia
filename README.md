
# Soroban Project

## Project Structure

This repository uses the recommended structure for a Soroban project:
```text
.
├── contracts
│   └── hello_world
│       ├── src
│       │   ├── lib.rs
│       │   └── test.rs
│       └── Cargo.toml
├── Cargo.toml
└── README.md
```

- New Soroban contracts can be put in `contracts`, each in their own directory. There is already a `hello_world` contract in there to get you started.
- If you initialized this project with any other example contracts via `--with-example`, those contracts will be in the `contracts` directory as well.
- Contracts should have their own `Cargo.toml` files that rely on the top-level `Cargo.toml` workspace for their dependencies.
- Frontend libraries can be added to the top-level directory as well. If you initialized this project with a frontend template via `--frontend-template` you will have those files already included.

Stellar Crowdfunding Workshop
Proyek DApp full-stack untuk platform crowdfunding di Stellar Soroban. Menggabungkan React/TypeScript frontend dengan Rust/Soroban kontrak pintar. Dibuat untuk edukasi 
(Stellar Indonesia Workshop Oktober 2025).

💡 Fitur & Konsep Inti
Logika On-Chain: Semua aturan (goal, deadline, refund) dijalankan oleh kontrak.

Token XLM: Menggunakan transfer XLM sebagai donasi.

Mekanisme Refund: Memungkinkan donatur menarik dana jika target gagal dicapai.

Pembelajaran: Rust, Soroban, dan state management on-chain.

🔗 Sumber Daya
Stellar Documentation

Soroban Examples

Risein & BlockDevId Community

Workshop Documentation
 39fc1bf76403452ccc2790bb96b19ed3b525d964
