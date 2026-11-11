---
layout: '../../layouts/BlogPost.astro'
title: 'Transformasi Digital Uji Riksa'
date: '2026-11-11'
description: 'Slide materi poin-poin yang akan disampaikan pada Presentasi 10 menit.'
tags: ['field-notes', 'methodology', 'monoceros']
---

Berikut desain presentasi 10 menit yang saya rancang untuk Anda, memanfaatkan posisi Anda sebagai *researcher* CS untuk memberi sudut pandang teknis yang kredibel tanpa mendominasi domain audiens.

---

## Struktur Presentasi (10 Slide, ±1 menit/slide)

### Slide 1 — Hook: "Angka yang Tidak Bisa Diabaikan"

**Konten:**
- 319.224 klaim kecelakaan kerja, **9.834 kematian** (data Menaker 2025)
- 250.000+ unit alat wajib riksa uji berkala
- Pertanyaan pemantik: *"Apakah cara kita menguji sudah secepat laju risikonya?"*

**Catatan presentasi:** Buka dengan data, bukan definisi. Audiens sudah tahu apa itu riksa uji — mereka butuh *urgensi*, bukan pengenalan.

---

### Slide 2 — Problem Statement: "Bottleneck Proses Manual"

**Konten (3 poin saja):**
1. **Administrasi**: Pencatatan manual → human error, dokumen tercecer, verifikasi lambat
2. **Reaktivitas**: Pengujian dilakukan *setelah* alat sudah beroperasi → risiko sudah berjalan
3. **Fragmentasi**: Data tersebar di banyak PJK3, tidak ada *single source of truth*

**Catatan:** Frame sebagai *systems problem* — ini bahasa yang natural bagi Anda sebagai CS researcher.

---

### Slide 3 — Framework: "3 Lapis Transformasi Digital"

**Konten (diagram 3 layer):**

| Layer | Fungsi | Teknologi |
|-------|--------|-----------|
| **Data Acquisition** | Pengumpulan data kondisi alat | Sensor IoT, NDT digital, *computer vision* |
| **Intelligence** | Analisis & prediksi | ML models, *predictive maintenance*, anomaly detection |
| **Ecosystem** | Orkestrasi & kepatuhan | Platform terpusat (SIK3/TemanK3), *digital certificate* |

**Catatan:** Ini slide "peta" — audiens akan kembali ke sini secara mental selama presentasi.

---

### Slide 4 — Layer 1: IoT & Sensorika

**Konten:**
- Sensor tekanan, getaran, suhu → transmisi *real-time* ke dashboard
- **Data**: Rata-rata waktu transmisi 1,8 detik (prototipe ESP32 + cloud, studi Universitas Pahlawan)
- Analogi: "Dari inspeksi *snapshot* → *continuous monitoring*"
- Contoh: Bejana tekan dengan sensor *real-time* → deteksi *pressure anomaly* sebelum *threshold* terlampaui

**Catatan:** Audiens profesional riksa uji akan langsung melihat relevansi dengan NDT dan *load test*. Tekankan bahwa IoT **melengkapi**, bukan menggantikan, pengujian periodik.

---

### Slide 5 — Layer 2: AI & Machine Learning

**Konten:**
- **Predictive Maintenance**: Random Forest → akurasi 98,47% klasifikasi kondisi *normal/anomaly/failure* (tesis generator set)
- **Anomaly Detection**: Deteksi *pattern* degradasi sebelum kegagalan
- **Computer Vision**: Inspeksi visual otomatis (retak, korosi, keausan)
- **Data**: 73% reduksi *near-miss incidents*, 75% penurunan waktu respons darurat (trial 6 bulan, 3 site manufaktur)

**Catatan:** Ini "jurus" Anda sebagai CS researcher — tunjukkan *method* (algoritma, akurasi) karena audiens akademis akan menghargai rigor teknis.

---

### Slide 6 — Layer 3: Platform & Ekosistem Digital

**Konten:**
- **TemanK3 / SIK3 Kemnaker**: Platform terpusat untuk pencatatan, verifikasi, dan penerbitan dokumen
- **Desember 2025**: Seluruh dokumen K3 (sertifikat, SKP, lisensi) resmi beralih ke format digital
- **Konsep Risk-Based Inspection Period**: Interval riksa uji dinamis berdasarkan *risk score* alat, bukan satu ukuran untuk semua
- **Digital Certificate**: Terintegrasi, *tamper-proof*, dapat diverifikasi online

**Catatan:** Ini poin *policy* — tunjukkan bahwa transformasi ini bukan wacana, sudah diimplementasikan oleh Kemnaker.

---

### Slide 7 — Studi Kasus: "Dari Teori ke Lapangan"

**Konten:**
- **PT X (Sektor Energi, Kalimantan Timur)**:
  - DNP berkala pada boiler & *heat exchanger*
  - Hasil: **Zero fatality** + efisiensi downtime **+18%**
  - Pencatatan digital via SIK3 Kemnaker
- **Prototipe IoT K3 (Pulogadung, Jakarta)**:
  - Sensor gas, suhu, detak jantung + ESP32 + cloud
  - Peringatan dini otomatis, dashboard *real-time*

**Catatan:** Satu studi kasus industri + satu prototipe akademis → menunjukkan spektrum dari *pilot* ke *production*.

---

### Slide 8 — Tantangan & Hambatan

**Konten (jujur, tidak over-optimistic):**

| Tantangan | Detail |
|-----------|--------|
| **Kesiapan SDM** | PJK3 kecil belum punya *capability* data engineering |
| **Interoperabilitas** | Standar data antar-PJK3 belum seragam |
| **Regulasi** | Permenaker 11/2026 masih dalam harmonisasi; status Permenaker 8/2020 belum konsisten |
| **Biaya awal** | Sensor + infrastruktur IoT → *capex* signifikan untuk PJK3 skala kecil |
| **Trust** | Hasil AI/ML harus *explainable* untuk diterima secara hukum |

**Catatan:** Slide ini penting untuk kredibilitas. Audiens akademis menghargai *critical perspective*, bukan *vendor pitch*.

---

### Slide 9 — Roadmap: "3 Fase Implementasi"

**Konten (timeline horizontal):**

```
Fase 1 (0-1 thn)          Fase 2 (1-3 thn)           Fase 3 (3-5 thn)
─────────────────────────────────────────────────────────────────────────
Digitalisasi pencatatan    IoT + predictive            Autonomous
& e-sertifikat             maintenance per alat        inspection (drone/robot)
                          + risk-based scheduling     + full digital twin
```

**Catatan:** Tunjukkan bahwa ini *incremental*, bukan *big bang*. Audiens profesional akan lebih percaya pada roadmap realistis.

---

### Slide 10 — Closing: "Kolaborasi yang Dibutuhkan"

**Konten:**
- Riksa uji digital bukan soal *mengganti* ahli K3, tapi *memberi superpower* pada ahli K3
- **Call to action** untuk audiens:
  - Dosen → riset metodologi & validasi model
  - Praktisi PJK3 → *pilot* implementasi & *ground truth data*
  - Regulator → kerangka hukum untuk *AI-assisted inspection*
- Penutup: *"Transformasi digital bukan tujuan — keselamatan pekerja adalah tujuan. Teknologi adalah jalannya."*

---

## Tips Eksekusi (10 Menit)

| Aspek | Saran |
|-------|-------|
| **Slide** | Maksimal 6-8 baris per slide; gunakan diagram, bukan paragraf |
| **Narasi** | Anda = "jembatan" antara CS dan K3. Jangan menjelaskan *apa* riksa uji (mereka sudah tahu), fokus pada *bagaimana teknologi mengubah prosesnya* |
| **Pacing** | Slide 1-2 cepat (2 menit total), Slide 3-6 inti (4 menit), Slide 7-10 penutup (4 menit) |
| **Q&A prep** | Siapkan jawaban untuk: "Apakah AI bisa menggantikan inspektur?" → *Tidak, AI adalah decision support, bukan decision maker. Validitas hukum tetap pada ahli bersertifikat.* |
| **Visual** | Slide 3 (framework 3 layer) dan Slide 9 (roadmap) layak dibuat sebagai diagram visual yang kuat — dua slide ini adalah "takeaway" utama |

---

Mau saya bantu detailkan salah satu slide tertentu, atau buatkan *speaker notes* per slide?

