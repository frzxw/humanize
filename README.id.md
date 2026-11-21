# humanize

[English](README.md)

[![skills.sh](https://skills.sh/b/frzxw/humanize)](https://skills.sh/frzxw/humanize)

Skill yang membersihkan jejak tulisan AI, dalam bahasa Inggris dan bahasa Indonesia.

Skill humanizer lain mengurus bahasa Inggris. Skill ini juga mengurus kegagalan yang muncul saat model menulis bahasa Indonesia: struktur kalimat Inggris, frasa formal yang kosong, dan kata kerja yang tertimbun di bawah "melakukan".

Instruksinya ada di [skills/humanize/SKILL.md](skills/humanize/SKILL.md): 40 pola, mode deteksi dan mode sunting, plus catatan singkat tentang cara memakainya di chat dan di repositori.

## Pasang

Dari proyek yang ingin dipasangi skill ini, dengan Node.js 22.20 atau yang lebih baru:

```bash
npx skills add frzxw/humanize
```

CLI akan menanyakan agen mana yang dipakai. Untuk melewati pertanyaan itu:

```bash
npx skills add frzxw/humanize --skill humanize -a claude-code -a cursor -a codex -y
```

Tambahkan `-g` kalau skill ini dipakai di semua proyek di komputer yang sama.

## Pasang manual

Salin folder [skills/humanize](skills/humanize) ke lokasi yang dibaca agen.

| Agen | Dalam satu proyek | Untuk semua proyek |
| --- | --- | --- |
| Claude Code | `.claude/skills/humanize` | `~/.claude/skills/humanize` |
| Cursor | `.agents/skills/humanize` | `~/.cursor/skills/humanize` |
| Codex | `.agents/skills/humanize` | `~/.codex/skills/humanize` |

Cursor juga membaca `.cursor/skills/humanize` di dalam proyek. Codex juga membaca `~/.agents/skills/humanize`.

## Sebelum dan sesudah

Bahasa Inggris. Fakta di versi pertama: halaman tagihan sudah tayang, dan orang bisa mengunduh 12 tagihan terakhir sebagai PDF.

Before:

> We are thrilled to announce that the new billing page is live, marking a pivotal moment in our journey. It is not just a page, it is a clearer way to see invoices. Users can download the last 12 invoices as PDF.

After:

> The new billing page is live. Users can download the last 12 invoices as PDF.

Bahasa Indonesia. Faktanya sama.

Sebelum:

> Perlu diketahui bahwa pada akhirnya tim kami telah melakukan peluncuran halaman tagihan baru di mana pengguna dapat melakukan pengunduhan 12 tagihan terakhir dalam rangka untuk meningkatkan pengalaman di era digital saat ini.

Sesudah:

> Halaman tagihan baru sudah tayang. Pengguna bisa mengunduh 12 tagihan terakhir.

## Yang membedakan

26 pola pertama berasal dari [blader/humanizer](https://github.com/blader/humanizer) oleh Siqi Chen, yang merangkum [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) di Wikipedia. Pola selanjutnya berasal dari [petergyang/no-ai-slop](https://github.com/petergyang/no-ai-slop) oleh Peter Yang.

Enam pola ditulis untuk skill ini:

- 28, struktur yang berlebihan
- 35, panjang jawaban yang tidak sesuai pertanyaan
- 37, bahasa Indonesia yang masih berstruktur Inggris
- 38, frasa Indonesia yang kosong
- 39, mengumumkan pekerjaan alih-alih mengerjakannya
- 40, detail yang diada-adakan

Bagian bahasa Indonesia ditulis untuk bahasa Indonesia, mengikuti cara orang menulis bahasa itu. Skill ini juga menjelaskan pemakaiannya di balasan chat dan di teks repositori: mulai dari keputusan, satu topik per pesan, dan pesan commit serta merge tanpa em dash sebagai engsel kalimat.

## Kontribusi

Usulan pola, tambahan bahasa, dan laporan bug lewat [CONTRIBUTING.md](CONTRIBUTING.md). Kode etik komunitas memakai [Contributor Covenant 2.1](CODE_OF_CONDUCT.md).

## Kredit

- Siqi Chen, [blader/humanizer](https://github.com/blader/humanizer), MIT
- Peter Yang, [petergyang/no-ai-slop](https://github.com/petergyang/no-ai-slop), MIT
- Kontributor Wikipedia, [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)

Teks lisensi kedua proyek hulu ada di [skills/humanize/licenses](skills/humanize/licenses). Repositori ini berlisensi MIT. Lihat [LICENSE](LICENSE) dan [NOTICE](NOTICE). Pemberitahuan yang sama ada di [skills/humanize/LICENSE](skills/humanize/LICENSE), jadi salinan hasil instalasi tetap membawanya.

## Dibuat oleh Fariz Wibisono

Saya menulis dan membangun di depan umum, dalam bahasa Inggris dan bahasa Indonesia.

- Situs: [frzxw.me](https://frzxw.me)
- X: [@frzwibisono](https://x.com/frzwibisono)
- LinkedIn: [frzxw](https://www.linkedin.com/in/frzxw)
- GitHub: [frzxw](https://github.com/frzxw)
