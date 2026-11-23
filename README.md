# AI Agent Skills untuk Studi Kasus Magang

Repository ini berisi **AI Agent Skills** yang dirancang untuk menggantikan atau membantu aktivitas repetitif pada 5 studi kasus magang. Skills ini mengikuti format standar Grok / agentskills.io (SKILL.md + resources).

## Cara Menggunakan

1. Clone atau download repository ini.
2. Letakkan folder skill yang diinginkan ke direktori skills agent Anda (contoh: `~/.grok/skills/` atau sesuai platform).
3. Agent akan otomatis mendeteksi skill berdasarkan `description` di frontmatter SKILL.md.
4. Trigger dengan kata kunci terkait jobdesk (lihat masing-masing skill).

## Identifikasi Jobdesk & Aktivitas Repetitif yang Bisa Digantikan AI

### 1. Magang Administrasi Perkantoran Dinas Pemerintahan Daerah
**Jobdesk umum:**
- Pengelolaan surat masuk/keluar (disposisi, numbering, distribusi)
- Kearsipan fisik & digital
- Penyusunan notulensi rapat & laporan kegiatan
- Pengelolaan agenda pimpinan & undangan
- Administrasi kepegawaian ringan (rekap absensi, data pegawai)
- Pembuatan surat resmi (nota dinas, surat edaran, undangan)

**Aktivitas repetitif yang cocok diganti AI:**
- Drafting surat resmi sesuai format dinas (kop, nomor, perihal, tembusan)
- Ringkasan notulensi rapat dari catatan/transkrip
- Klasifikasi & tagging arsip
- Pembuatan agenda harian/mingguan
- Rekap data sederhana & template laporan
- Checklist kelengkapan dokumen

**Skill:** `admin-perkantoran-dinas`

### 2. Magang di Klinik Dokter — Bagian Registrasi & Anamnesa
**Jobdesk umum:**
- Registrasi pasien baru & lama (data demografi, asuransi/BPJS)
- Anamnesa awal (keluhan utama, riwayat penyakit, alergi, obat)
- Penjadwalan konsultasi/dokter
- Input rekam medis awal
- Verifikasi identitas & dokumen

**Aktivitas repetitif yang cocok diganti AI:**
- Guided conversation untuk anamnesa terstruktur (SOAP-like)
- Ekstraksi data pasien dari percakapan/teks
- Validasi kelengkapan data registrasi
- Generate ringkasan anamnesa untuk dokter
- Reminder & konfirmasi jadwal
- Template form anamnesa berdasarkan keluhan

**Skill:** `klinik-registrasi-anamnesa`

### 3. Magang di Digital Marketing Agency
**Jobdesk umum:**
- Content calendar & scheduling social media
- Draft caption, ad copy, blog brief
- Keyword research & competitor snapshot
- Weekly/monthly performance report
- A/B testing idea generation
- Email newsletter draft

**Aktivitas repetitif yang cocok diganti AI:**
- Generate multiple caption variations + hashtag
- Buat content calendar dari brief klien
- Ringkasan laporan analytics (CTR, engagement, ROAS)
- Keyword clustering & search intent
- Draft email sequence
- Competitor content audit ringkas

**Skill:** `digital-marketing-agency`

### 4. Magang di Perusahaan Sawit — Bagian HRD
**Jobdesk umum:**
- Administrasi kepegawaian (absensi, cuti, BPJS)
- Recruitment support (screening CV, jadwal interview)
- Onboarding dokumen
- Rekap data karyawan kebun/mill
- Surat keterangan & SK ringan
- Hubungan industrial dasar

**Aktivitas repetitif yang cocok diganti AI:**
- Screening CV berdasarkan kriteria lowongan
- Draft offer letter / perjanjian kerja
- Rekap absensi & cuti
- Generate checklist onboarding
- Template surat keterangan kerja / rekomendasi
- Ringkasan data karyawan untuk laporan HRD

**Skill:** `hrd-perusahaan-sawit`

### 5. Magang di Bank — Bagian Kredit
**Jobdesk umum:**
- Penerimaan & checklist dokumen pengajuan kredit
- Analisis laporan keuangan sederhana (rasio)
- Penyusunan nota analisa kredit (NAC) draft
- Verifikasi data debitur
- Follow-up kelengkapan dokumen
- Monitoring kolektibilitas ringan

**Aktivitas repetitif yang cocok diganti AI:**
- Checklist kelengkapan dokumen kredit (KPR, KUR, modal kerja)
- Perhitungan rasio keuangan otomatis dari data laporan
- Draft struktur nota analisa (aspek 5C/7P)
- Template surat permintaan kelengkapan dokumen
- Ringkasan risiko awal
- Generate tabel perbandingan plafon & angsuran

**Skill:** `bank-kredit-analisa`

## Struktur Repository

```
ai-agent-skills-magang/
├── README.md
├── admin-perkantoran-dinas/
│   └── SKILL.md
├── klinik-registrasi-anamnesa/
│   └── SKILL.md
├── digital-marketing-agency/
│   └── SKILL.md
├── hrd-perusahaan-sawit/
│   └── SKILL.md
└── bank-kredit-analisa/
    └── SKILL.md
```

## Cara Upload ke GitHub (Public)

1. Buat repository baru di GitHub (centang **Public**).
2. Upload folder ini, atau:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: AI Agent Skills for 5 internship cases"
   git branch -M main
   git remote add origin https://github.com/USERNAME/REPO-NAME.git
   git push -u origin main
   ```
3. Pastikan repository **Public** agar bisa diakses siapa saja.

## Catatan

- Skills ini bersifat **template generik**. Sesuaikan dengan SOP instansi/perusahaan masing-masing (format surat, form anamnesa, kebijakan kredit, dll).
- AI Agent **membantu**, bukan menggantikan tanggung jawab manusia (terutama di klinik & bank yang sensitif data & keputusan).
- Selalu review output AI sebelum digunakan resmi.
- Data pribadi pasien/debitur harus di-handle sesuai UU PDP & kerahasiaan bank.

Dibuat untuk keperluan studi kasus magang / tugas kampus.
