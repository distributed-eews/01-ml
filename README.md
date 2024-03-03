# Deploy Queue dengan Docker Compose

## Overview

Layanan queue adalah layanan yang berfungsi untuk melakukan pooling data dan mengatasi data missing.

## Requirements

- VM dengan Docker dan Docker Compose terinstal.

## Deployment Steps

1. **Konfigurasi Queue**

   - Pastikan environment variables pada `docker-compose.yaml` sudah benar.

2. **Menjalankan Queue**

   - Navigasikan ke direktori tempat file `docker-compose.yaml` berada.
   - Jalankan perintah berikut untuk mendeploy Queue:

     ```sh
     docker-compose up -d
     ```

   - Periksa status container untuk memastikan layanan berjalan dengan baik:

     ```sh
     docker-compose ps
     ```

## Catatan

- Lihat `docker-compose.double.yaml` untuk mendeploy lebih dari 1 layanan queue dalam 1 vm.
