# Mimariye Genel Bakış

<details open>
<summary><strong>🇹🇷 Türkçe</strong></summary>
<br>

Bu sayfa, **localde çalışıyordu** sitesinin mimarisini, ana bileşenlerini ve bu bileşenlerin birbiriyle olan ilişkilerini açıklamaktadır.

---

## 🗂️ Projeye Genel Bakış

*localde çalışıyordu*, **Jekyll** tabanlı bir statik websitesidir. Yazar Markdown formatında bülten yazar; Jekyll bu dosyaları derleme aşamasında HTML'e dönüştürür ve ortaya sunucuya ihtiyaç duymayan, tamamen statik bir site çıkar. Site GitHub Pages üzerinde barındırılabilir.

---

## 🧱 Ana Bileşenler

| Bileşen | Teknoloji | Açıklama |
|---|---|---|
| İçerik Kaynağı | Markdown (`.md`) | Bültenler `_posts/` altında tarih önekli dosyalar olarak yazılır |
| Site Oluşturucu | Jekyll + Liquid | Markdown'ı HTML'e dönüştürür; şablon motoruyla layout ve değişkenleri birleştirir |
| Şablonlar | HTML + Liquid | `_layouts/default.html` (temel iskelet) ve `_layouts/post.html` (yazı görünümü) |
| Stil | Vanilla CSS | `assets/css/style.css` — CSS değişkenleriyle açık/koyu tema desteği |
| Bağımlılık Yönetimi | Bundler + Gemfile | Jekyll ve eklentilerinin sürümlerini sabitler |
| Eklentiler | `jekyll-feed` | Otomatik olarak `feed.xml` (RSS/Atom) üretir |
| Barındırma | GitHub Pages (opsiyonel) | `_site/` çıktısı doğrudan sunuluyor |

---

## 📁 Dizin Yapısı

```
localde-calisiyordu/
│
├── _posts/              # Bülten içerikleri — her dosya bir sayı
│   └── YYYY-MM-DD-slug.md
│
├── _layouts/            # Sayfa şablonları (Liquid + HTML)
│   ├── default.html     # Temel iskelet: <head>, header, footer, dark mode toggle
│   └── post.html        # Bülten sayfası; default'u miras alır
│
├── assets/
│   └── css/
│       └── style.css    # Tüm stiller; CSS değişkenleriyle açık/koyu tema
│
├── docs/                # Proje dokümantasyonu (bu dosya dahil)
│
├── index.md             # Ana sayfa — site.posts döngüsüyle bülten arşivi
├── _config.yml          # Jekyll yapılandırması (başlık, URL, eklentiler)
├── Gemfile              # Ruby bağımlılıkları
└── _site/               # Jekyll'ın ürettiği çıktı (versiyon kontrolüne dahil edilmez)
```

---


## 🗂️ Project Overview

*localde çalışıyordu* is a **Jekyll**-based static website. The author writes newsletters in Markdown; Jekyll transforms those files into HTML at build time, producing a fully static site that requires no server. The site can be hosted on GitHub Pages.

---

## 🧱 Main Components

| Component | Technology | Description |
|---|---|---|
| Content Source | Markdown (`.md`) | Newsletters are written as date-prefixed files under `_posts/` |
| Site Generator | Jekyll + Liquid | Converts Markdown to HTML; merges layouts and variables via its templating engine |
| Templates | HTML + Liquid | `_layouts/default.html` (base skeleton) and `_layouts/post.html` (post view) |
| Styling | Vanilla CSS | `assets/css/style.css` — light/dark theme via CSS custom properties |
| Dependency Management | Bundler + Gemfile | Pins versions of Jekyll and plugins |
| Plugins | `jekyll-feed` | Automatically generates `feed.xml` (RSS/Atom) |
| Hosting | GitHub Pages (optional) | The `_site/` output is served directly |

---

## 📁 Directory Structure

```
localde-calisiyordu/
│
├── _posts/              # Newsletter content — one file per issue
│   └── YYYY-MM-DD-slug.md
│
├── _layouts/            # Page templates (Liquid + HTML)
│   ├── default.html     # Base skeleton: <head>, header, footer, dark mode toggle
│   └── post.html        # Newsletter page; inherits default
│
├── assets/
│   └── css/
│       └── style.css    # All styles; light/dark theme via CSS variables
│
├── docs/                # Project documentation (including this file)
│
├── index.md             # Homepage — newsletter archive via site.posts loop
├── _config.yml          # Jekyll config (title, URL, plugins)
├── Gemfile              # Ruby dependencies
└── _site/               # Jekyll's generated output (not tracked in version control)
```

</details>