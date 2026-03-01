# Geliştirme Akışı

<details open>
<summary><strong>🇹🇷 Türkçe</strong></summary>
<br>

Bu belge, **localde çalışıyordu** projesine katkıda bulunmak için izlenmesi gereken geliştirme süreçlerini, standartları ve iş akışını açıklar.

---

## 🚀 Başlarken

### Ön Koşullar

- Git (lokal makinenizde kurulu olmalı)
- Ruby (3.0 veya üzeri)
- Bundler

### Kurulum

```bash
git clone https://github.com/Bilgisayar-Kavramlari-Toplulugu/localde-calisiyordu.git
cd localde-calisiyordu
bundle install
bundle exec jekyll serve
```

Tarayıcınızdan `http://localhost:4000` adresine giderek siteyi görüntüleyebilirsiniz.

---

## 🌿 Branch Stratejisi

| Branch | Amaç |
|---|---|
| `main` | Yayınlanmış, stabil içerik. Doğrudan push yapılmaz. |
| `feature/...` | Yeni özellikler veya içerikler için kısa ömürlü branch'ler |

Branch isimlendirme kuralı:
```
feature/<issue-no>-<kisa-aciklama>
# Örnek: feature/12-add-feb-3-newsletter
```

---

## ✍️ Yeni Bülten Sayısı Ekleme

1. `main`'den yeni bir branch oluşturun:
   ```bash
   git checkout -b feature/<issue-no>-bulten-<sayi>
   ```
2. `_posts/` altına `YYYY-MM-DD-slug.md` formatında dosya oluşturun:
   ```yaml
   ---
   layout: post
   title: "Bülten #N: Başlık"
   date: YYYY-MM-DD
   ---
   ```
3. Yerel önizleme yapın: `bundle exec jekyll serve`
4. Commit atın ve PR açın

---

## 🔄 Pull Request Süreci

1. PR açarken ilgili issue'yu referans gösterin (`Closes #123`)
2. PR açıklamasında içeriği kısaca özetleyin
3. Proje lideri veya en az bir takım üyesi tarafından incelenmeli
4. Onay sonrası `main`'e birleştirilir; GitHub Pages otomatik olarak güncellenir

---

## 📝 Kod ve İçerik Standartları

- Commit mesajları açıklayıcı ve Türkçe veya İngilizce olabilir
- Markdown dosyalarında front matter eksiksiz olmalı (`layout`, `title`, `date`)
- `_site/` klasörü versiyon kontrolüne dahil edilmemelidir (`.gitignore`'da tanımlı)
- Dokümantasyon değişikliklerinde (bu klasör) ilgili Wiki sayfası da güncellenmelidir

---

## 🧪 Test

```bash
# Sitenin hatasız derlendiğini doğrula
bundle exec jekyll build

# Yerel önizleme (canlı yenileme ile)
bundle exec jekyll serve
```

</details>

<details>
<summary><strong>🇬🇧 English</strong></summary>
<br>

This document describes the development processes, standards, and workflow for contributing to the **localde çalışıyordu** project.

---

## 🚀 Getting Started

### Prerequisites

- Git (installed on your local machine)
- Ruby (3.0 or higher)
- Bundler

### Setup

```bash
git clone https://github.com/Bilgisayar-Kavramlari-Toplulugu/localde-calisiyordu.git
cd localde-calisiyordu
bundle install
bundle exec jekyll serve
```

Access the site at `http://localhost:4000` in your browser.

---

## 🌿 Branching Strategy

| Branch | Purpose |
|---|---|
| `main` | Published, stable content. No direct pushes. |
| `feature/...` | Short-lived branches for new features or content |

Branch naming convention:
```
feature/<issue-no>-<short-description>
# Example: feature/12-add-feb-3-newsletter
```

---

## ✍️ Adding a New Newsletter Issue

1. Create a new branch from `main`:
   ```bash
   git checkout -b feature/<issue-no>-newsletter-<number>
   ```
2. Create a file in `_posts/` using the `YYYY-MM-DD-slug.md` format:
   ```yaml
   ---
   layout: post
   title: "Newsletter #N: Title"
   date: YYYY-MM-DD
   ---
   ```
3. Preview locally: `bundle exec jekyll serve`
4. Commit and open a PR

---

## 🔄 Pull Request Process

1. Reference the related issue when opening a PR (`Closes #123`)
2. Briefly summarize the content in the PR description
3. Must be reviewed by the project lead or at least one team member
4. After approval, merged to `main`; GitHub Pages updates automatically

---

## 📝 Code & Content Standards

- Commit messages can be in Turkish or English; keep them descriptive
- Markdown files must have complete front matter (`layout`, `title`, `date`)
- The `_site/` directory must not be tracked in version control (defined in `.gitignore`)
- Documentation changes should also update the relevant Wiki page

---

## 🧪 Testing

```bash
# Verify the site builds without errors
bundle exec jekyll build

# Local preview (with live reload)
bundle exec jekyll serve
```

</details>