
## 📌 Introduce
<div align="center">
  <img src="public/favicon.png" alt="vharasc">
  
![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-0.121.2-009688?style=for-the-badge&logo=fastapi)
![Vercel](https://img.shields.io/badge/Vercel-Deploy-black?style=for-the-badge&logo=vercel)
![Redis](https://img.shields.io/badge/Redis-Caching-red?style=for-the-badge&logo=redis)

**Rest-API**

Project ini adalah **Rest-like API / Wrapper API** yang melakukan scraping data dari berbagai situs sumber platform populer di Indonesia secara *real-time*. Dibangun dengan **FastAPI**, API ini cepat, *asynchronous*.

[![Live Demo](https://img.shields.io/badge/🚀%20Live%20Demo-Click%20Here-success?style=for-the-badge)](https://www.vharasc.my.id/)
[![Documentation](https://img.shields.io/badge/📘%20Documentation-API%20Docs-blue?style=for-the-badge)](https://api.vharasc.my.id/docs)

---

</div>

## 🌐 Supported Platforms

| Platform | Status | Route | Endpoint | Info |
| :--- | :---: | :--- | :--- | :--- |
| Oploverz | 🟢 | /oploverz | 26 | Anime |
| Samehadaku | 🟢 | /samehadaku | 16 | Anime |
| Kusonime | 🟢 | /kusonime | 11 | Anime |
| Anoboy | 🟢 | /anoboy | 29 | Anime |
| LayarAnime | 🔴 | - | - | - |
| NimeGami | 🟢 | /nimegami | 11 | Anime |
| Nekopoi | 🟢 | /nekopoi | 13 | H-Nime, JAV, 2D, 3D, Cosplay |
| Komiku | 🟢 | /komiku | 11 | Manga, Manhua, Manhwa |
| Doujindesu | 🟢 | /doujindesu | 11 | Manga, Manhwa, Manhua, Eroge |
| Dojing | 🟢 | /adultcomic_v1 | 8 | Comic, Eroge, Manga |
| KomikDewasa | 🟢 | /adultcomic_v2 | 9 | Baca Kitab Suci |
| PixHentai | 🟢 | /adultcomic_v3 | 7 | Baca Kitab Suci |
| AnimeKompi | 🟢 | /animekompi | 25 | Anime |
| AniChin | 🟢 | /anichin | 26 | Donghua |
| MangaKita | 🟢 | /mangakita | 12 | Comic |
| CrotPedia | 🔴 | - | - | - |
| KomikIndo | 🟢 | /komikindo | 20 | Comic |
| ShiroDoujin | 🟢 | /shirodoujin | 18 | Manhwa, Manga, Doujinshi |
| KomikKita | 🟢 | /komikkita | 18 | Manhwa, Manga, Manhua |
| AnimeBagus | 🔴 | - | - | - |
| DonghuaFilm | 🟢 | /donghuafilm | 25 | Donghua |

---

## 🔥 Features

*   **🛡️ Anti-Bot Bypass:** Menggunakan `Cloudscraper`, `httpx[2]` & `Curl_cffi` untuk menembus proteksi Cloudflare.
*   **🔑 Smart Tiered Rate Limiting:** Sistem manajemen kuota request berbasis API Key (Guest, Free, Admin, Dev, Owner).
*   **🚀 Fast Response:** Dibangun di atas FastAPI + Uvicorn.
*   **💾 Redis Caching:** Integrasi opsional dengan Redis untuk performa maksimal.
*   **📝 IP Logging & Stats:** Middleware canggih untuk mencatat trafik, mendeteksi abuse, dan memblokir IP nakal.
*   **📖 Auto Documentation:** Swagger UI (`/docs`) dan ReDoc interaktif.

---

## 🔑 API Key System

Opsional...

1.  **Guest (Tanpa Key):** Limit 30 request/menit. Cocok untuk testing.
2.  **Free Tier:** Limit 100 request/menit + 5000 request/bulan.
3.  **Admin/Dev/Owner:** Unlimited Power!

---

## 🤖 Usage

baseurl = `https://www.vharasc.my.id`
```
curl {baseurl}/api/v1/{platform}/{endpoint}/{slug}
```

---

## ⚠️ Disclaimer

Project ini dibuat untuk **tujuan edukasi** dan pembelajaran tentang web scraping & API development.
*   Disini, setiap API tersedia secara <span class="highlight">gratis</span> untuk digunakan tanpa embel-embel <span class="highlight">apikey</span>, <span class="highlight">premium</span>, <span class="highlight">membership</span>, dan istilah lainnya, kamu nggak perlu spend money <span class="highlight">sepeser pun</span>. Namun, ada pula yang perlu kamu diketahui bahwa, semua API yang tersedia bersifat <span class="highlight">unofficial</span> dalam kata lain, ini adalah Rest-like API atau API Wrapper
*   Sehingga, suatu waktu API bisa mati kapapun jika <span class="highlight">struktur HTML</span> sumber berubah. Kami tidak selalu memantau perkembangan situs sumber yang ada, untuk itu, kami perlu kontribusi dari kamu jika menemukan <span class="highlight">bug</span> atau <span class="highlight">error</span> pada <span class="highlight">API</span> atau <span class="highlight">endpoint</span> yang tersedia.</p>
*   Kemudian, kami tidak menyarankan kamu mempergunakan layanan kami untuk tujuan <span class="highlight">KOMERSIL</span>, gunakan layanan kami hanya sebatas <span class="highlight">HOBI</span> ataupun <span class="highlight">PEMBELAJARAN</span> semata, kami tidak akan <span class="highlight">BERTANGGUNG JAWAB</span> atas apa yang akan terjadi dimasa mendatang jika kamu bersiteguh <span class="highlight">abai</span> dengan saran dari kami

---

## 📄 Changelog

```json
changelogs = [
    {
        "date": "2026-02-22",
        "changes": [
            "Update: Anoboy",
            "Add: New Endpoint [/update, /latest, /popular, /rating, /ongoing, /completed, /upcoming, /movie, /recommendation, /season-list, /studio-list, /top-weekly, /top-monthly, /top-alltime, /director/{director}, /studio/{studio}, /producer/{producer}, /cast/{cast}, /season/{season}]"
        ]
    },
    {
        "date": "2026-02-19",
        "changes": [
            "Update: Oploverz",
            "Add: New Endpoint [/popular-today, /recommendation, /latest, /ongoing, /completed, /upcoming, /popular, /rating, /movie, /list-genre, /list-studio, /list-season, /genre/{genre}, /studio/{studio}, /season/{season}, /cast/{cast}, /director/{director}]",
            "Remove: [/home]"
        ]
    },
    {
        "date": "2026-02-18",
        "changes": [
            "Remove: AnimeBagus, CrotPedia, LayarAnime",
            "Update: UI/UX Enchanted!"
        ]
    },
    {
        "date": "2026-02-13",
        "changes": [
            "New: Platform DonghuaFilm [Complete Endpoint]",
            "Adjust: Global Proxy Rotate",
            "Add: Anichin [/latest, /popular, /rating, /movie] endpoints",
            "Update: Platforms Data for AniChin"
        ]
    },
    {
        "date": "2026-02-12",
        "changes": [
            "New: Platform KomikKita [Complete Endpoint]",
            "Add: KomikKita Image Proxy (BunnyCDN & WP)",
            "Fix: Global Image Proxy consistency",
            "Update: Platform Komiku [5 New Endpoints]",
            "Add: Komiku Random, Latest, New, Popular, and Genre Detail",
            "Fix: Komiku [/read]",
            "Fix: Komiku Parser item mapping (Title, Thumb, Info, Chapters, Type, Genre, Synopsis)",
            "New: Platform AnimeBagus [Complete Endpoint]",
            "Add: AnimeBagus Parallel Episode Fragment Fetching",
            "Add: AnimeBagus Path-based slug for Watch endpoint consistency",
            "Add: Samehadaku [/schedule]",
            "Fix: AnimeBagus [/watch]"
        ]
    },
    {
        "date": "2026-02-11",
        "changes": [
            "New: Platform ShiroDoujin [Complete Endpoint]",
            "New: Platform Samehadaku [Complete Endpoint] Robust Version!"
        ]
    },
    {
        "date": "2026-02-10",
        "changes": [
            "New: Platform KomikIndo [Complete Endpoint]",
            "Adjust: KomikIndo Parser Logic",
            "Fix: Komikindo [/project]",
            "Add: KomikIndo External Image Proxy",
            "Add: Margin News Letter"
        ]
    },
    {
        "date": "2026-02-09",
        "changes": [
            "New: Platform MangaKita [Complete Endpoint]",
            "New: Platform CrotPedia [Complete Endpoint]",
            "Fix: CrotPedia Parse Error",
            "Adjust: CrotPedia Parsing Method"
        ]
    },
    {
        "date": "2026-02-08",
        "changes": [
            "New: Platform AniChin [Complete Endpoint]"
        ]
    },
    {
        "date": "2026-02-07",
        "changes": [
            "New: Platform AnimeKompi [Complete Endpoint]",
            "New: Platform AdultComic V3 [Complete Endpoint]",
            "Adjust: Views layout for better mobile responsiveness",
            "Fix: Nekopoi search parsing error on page 2",
            "Add: Rate Limit headers (X-RateLimit-Limit, X-RateLimit-Remaining)"
        ]
    },
    {
        "date": "2026-02-06", 
        "changes": [
            "Fix: Anoboy search pagination loop",
            "Add: Endpoint /detail on Oploverz",
            "Adjust: Cloudscraper timeout increased to 15s",
            "Remove: Legacy Komiku parser logic"
        ]
    },
    {
        "date": "2026-02-05", 
        "changes": [
            "New: AdultComic V2 [Complete Endpoint]",
            "Fix: Anoboy search pagination loop",
            "Add: Endpoint /detail on Oploverz",
            "Adjust: Proxy Rotate Handlers",
            "Remove: Legacy Komiku parser logic",
            "Optimize: AdultComic V2 [Complete Endpoint]"
        ]
    },
    {
        "date": "2026-02-04", 
        "changes": [
            "Adjust: Proxy Rotate Handlers",
            "New: AdultComic V2 [adultcomic_v2/home]"
        ]
    },
    {
        "date": "2026-02-01", 
        "changes": [
            "Fix: Reverse Proxy Image > Oploverz & Komiku",
            "New: AdultComic V1 [Complete Endpoint]"
        ]
    },
]
```

---