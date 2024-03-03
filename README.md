# Deploy ML dengan Docker Compose

## Overview

Layanan ML adalah layanan yang berisi model machine learning.

## Requirements

- VM dengan Docker dan Docker Compose terinstal.
- Pastikan untuk membuka **port** yang dibutuhkan agar bisa diakses dari luar vm.

## Deployment Steps

1. **Konfigurasi ML**

   - Pastikan environment variables pada `docker-compose.yaml` sudah benar.

2. **Menjalankan ML**

   - Navigasikan ke direktori tempat file `docker-compose.yaml` berada.
   - Jalankan perintah berikut untuk mendeploy ML:

     ```sh
     docker-compose up -d
     ```

   - Periksa status container untuk memastikan layanan berjalan dengan baik:

     ```sh
     docker-compose ps
     ```

## Catatan

- Lihat `docker-compose.double.yaml` untuk mendeploy lebih dari 1 layanan queue dalam 1 vm.
