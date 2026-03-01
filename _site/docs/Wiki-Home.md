# localde çalışıyordu — Wiki

<details open>
<summary><strong>🇹🇷 Türkçe</strong></summary>
<br>

Bu alan, **localde çalışıyordu** projesinin yaşayan dokümantasyon merkezidir. Projenin mimarisi, tasarım kararları ve uzun vadeli bilgileri burada yer alacaktır.

👤 **Proje Lideri:** [@gecicidegisken](https://github.com/gecicidegisken)  
👥 **Takım:** [localde-calisiyordu Üyeleri](https://github.com/orgs/Bilgisayar-Kavramlari-Toplulugu/teams/localde-calisiyordu)

---

### 📖 Proje Nedir?

**localde çalışıyordu**, [Bilgisayar Kavramları Topluluğu](https://bilgisayarkavramlari.com) bünyesindeki Yazılım/Programlama grubunun haftalık haber bültenidir. Yazılım dünyasındaki güncel gelişmeler, topluluk içi haberler, ilginç projeler ve teknik okumalar Markdown formatında yazılıp Jekyll ile statik HTML olarak yayınlanır.

Site, yazarların teknik altyapıyla vakit kaybetmeden içerik üretmesine izin verecek şekilde kasıtlı olarak sade tutulmuştur: bir yazı eklemek için tek yapmanız gereken `_posts/` klasörüne yeni bir `.md` dosyası koymaktır.

---

### 🗺️ Sayfa Haritası

| Sayfa | Açıklama |
|---|---|
| [Mimariye Genel Bakış](./Architecture-Overview.md) | Jekyll tabanlı statik site altyapısı, dizin yapısı ve teknoloji seçimleri |
| [Geliştirme Akışı](./Development-Workflow.md) | Branch stratejisi, PR süreci ve kod standartları |
| [Proje Tanımı](./Project-Definition.md) | Projenin amacı, hedefleri ve kapsamı |
| [Takım Bilgileri](./Team.md) | Proje ekibi ve roller |
| [Doğrulanmış Commit Rehberi](./Verified-Commits-Guide.md) | Commit imzalama ve GPG kurulumu |

---

### 📝 Yeni İçerik Nasıl Eklenir?

1. `_posts/` klasörüne `YYYY-MM-DD-slug.md` formatında yeni bir dosya oluşturun
2. Dosyanın en üstüne front matter ekleyin:
   ```yaml
   ---
   layout: post
   title: "Bülten #N: Başlık"
   date: YYYY-MM-DD
   ---
   ```
3. İçeriği Markdown olarak yazın
4. `bundle exec jekyll serve` ile yerel önizleme yapın
5. PR açın → inceleme → `main`'e birleştirin

---

### 🔗 Faydalı Bağlantılar

- [GitHub Repository](https://github.com/Bilgisayar-Kavramlari-Toplulugu/localde-calisiyordu)
- [Issue Takip Panosu](https://github.com/Bilgisayar-Kavramlari-Toplulugu/localde-calisiyordu/issues)
- [Proje Panosu](https://github.com/Bilgisayar-Kavramlari-Toplulugu/localde-calisiyordu/projects)
- [Bilgisayar Kavramları Topluluğu](https://bilgisayarkavramlari.com)

</details>

<details>
<summary><strong>🇬🇧 English</strong></summary>
<br>

This is the living documentation hub for the **localde çalışıyordu** project. The project's architecture, design decisions, and long-term information reside here.

👤 **Project Lead:** [@gecicidegisken](https://github.com/gecicidegisken)  
👥 **Team:** [localde-calisiyordu Members](https://github.com/orgs/Bilgisayar-Kavramlari-Toplulugu/teams/localde-calisiyordu)

---

### 📖 What Is This Project?

**localde çalışıyordu** is a weekly newsletter by the Programming group of [Bilgisayar Kavramları Topluluğu](https://bilgisayarkavramlari.com) (Computer Concepts Community). Current developments in the software world, community news, interesting projects, and technical reads are written in Markdown and published as static HTML via Jekyll.

The site is intentionally kept simple so authors can focus on writing rather than infrastructure: adding a new issue only requires placing a new `.md` file in `_posts/`.

---

### 🗺️ Page Index

| Page | Description |
|---|---|
| [Architecture Overview](./Architecture-Overview.md) | Jekyll-based static site infrastructure, directory structure, and technology choices |
| [Development Workflow](./Development-Workflow.md) | Branching strategy, PR process, and coding standards |
| [Project Definition](./Project-Definition.md) | Purpose, goals, and scope of the project |
| [Team Information](./Team.md) | Project team and roles |
| [Verified Commits Guide](./Verified-Commits-Guide.md) | Commit signing and GPG setup |

---

### 📝 How to Add New Content

1. Create a new file in `_posts/` using the `YYYY-MM-DD-slug.md` format
2. Add front matter at the top of the file:
   ```yaml
   ---
   layout: post
   title: "Newsletter #N: Title"
   date: YYYY-MM-DD
   ---
   ```
3. Write the content in Markdown
4. Preview locally with `bundle exec jekyll serve`
5. Open a PR → review → merge to `main`

---

### 🔗 Useful Links

- [GitHub Repository](https://github.com/Bilgisayar-Kavramlari-Toplulugu/localde-calisiyordu)
- [Issue Tracker](https://github.com/Bilgisayar-Kavramlari-Toplulugu/localde-calisiyordu/issues)
- [Project Board](https://github.com/Bilgisayar-Kavramlari-Toplulugu/localde-calisiyordu/projects)
- [Computer Concepts Community](https://bilgisayarkavramlari.com)

</details>