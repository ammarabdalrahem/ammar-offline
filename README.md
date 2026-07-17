# عمّار غير متصل — Ammar Offline

Medium-style personal blog in Arabic (RTL) using the official [Thmanyah typeface](https://font.thmanyah.com/), built with Jekyll for GitHub Pages.

## Deploy to GitHub Pages (5 minutes)

1. Create a new repository on GitHub named `USERNAME.github.io` (replace `USERNAME` with your GitHub username).
2. Push this folder to it:

   ```bash
   cd arabic-blog
   git init
   git add .
   git commit -m "My Arabic blog"
   git branch -M main
   git remote add origin https://github.com/USERNAME/USERNAME.github.io.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main` / `(root)` → Save.
4. Your blog is live at `https://USERNAME.github.io` within a minute or two.

> To use a differently-named repo (e.g. `blog`), set `baseurl: "/blog"` in `_config.yml` and the site will be at `https://USERNAME.github.io/blog`.

## Rename the blog

Edit the top of `_config.yml`:

```yaml
title: مدونتي            # ← your blog name
tagline: أفكار وملاحظات شخصية
author: عمّار             # ← your name
```

## Write a new post

Add a Markdown file to `_posts/` named `YYYY-MM-DD-slug.md`:

```markdown
---
layout: post
title: عنوان المقال
subtitle: وصف قصير اختياري
---

نص المقال بالعربية...
```

Push it — GitHub rebuilds the site automatically.

## Add images to a post

Put the image in `assets/images/`, then in your Markdown:

```markdown
![وصف الصورة](/assets/images/my-photo.jpg)
```

## Visitor analytics (who visits, from which country)

1. Sign up free at [goatcounter.com](https://www.goatcounter.com) and pick a code (e.g. `ammar`).
2. Set it in `_config.yml`: `goatcounter: "ammar"`.
3. Push — your dashboard at `https://ammar.goatcounter.com` shows visits per page, country, browser, and referrer. No cookies, GDPR-friendly.

## Preview locally (optional)

```bash
gem install bundler
bundle install
bundle exec jekyll serve
# → http://localhost:4000
```

## Credits & Licenses

This project stands on the work of others — please keep this section if you reuse it:

**Font — خط ثمانية (Thmanyah Typeface)**
Designed and owned by [Thmanyah Company](https://company.thmanyah.com/) (شركة ثمانية للنشر والتوزيع). Official source: [font.thmanyah.com](https://font.thmanyah.com/). Free for personal and commercial use under the [Thmanyah font license](https://font.thmanyah.com/licenses). The three families self-hosted in `assets/fonts/` (Serif Display for headlines, Serif Text for article body, Sans for UI) remain © Thmanyah and are **not** covered by this repo's MIT license.

**Theme**
Custom-built for this blog with [Jekyll](https://jekyllrb.com/) (MIT). Layout and typography are inspired by the reading experience of [Medium](https://medium.com/) — no Medium code or assets are used. Theme code (layouts, includes, CSS) is released under the MIT License (see `LICENSE`): free to use, copy, and modify with attribution.

**Analytics**
Optional [GoatCounter](https://www.goatcounter.com/) — open-source, privacy-friendly web analytics.
