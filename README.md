# ✈️ My Travel Blog

A simple personal blog to keep loved ones updated while traveling. Built with [Astro](https://astro.build) and hosted on Vercel.

---

## 🚀 First-time setup

```bash
npm install
npm run dev       # opens at http://localhost:4321
```

Connect the repo to Vercel and it will auto-deploy on every push.

---

## ✍️ Writing a new post

Create a new `.md` file in `src/content/blog/`. Name it anything — e.g. `03-venice.md`.

```markdown
---
title: "Venice at dawn"
date: 2025-06-22
location: "Venice, Italy"
description: "Woke up early and had the canals to myself."
cover: "/images/venice-canal.jpg"
---

Your post content goes here. Write as much or as little as you want.

You can add photos anywhere with:

![Caption text](/images/your-photo.jpg)
```

### Frontmatter fields

| Field | Required | Description |
|-------|----------|-------------|
| `title` | ✅ | Post title |
| `date` | ✅ | Date in `YYYY-MM-DD` format |
| `location` | optional | Shown as 📍 on the post |
| `description` | optional | Short teaser shown on the homepage |
| `cover` | optional | Hero image at the top of the post |

---

## 📷 Adding photos

1. Drop the photo file into `public/images/`
2. Reference it in your markdown as `/images/your-photo.jpg`

**Tips for traveling:**
- Resize photos before adding them (aim for under 1–2 MB each) to keep the repo fast
- Or link directly to an iCloud shared album / Google Photos URL instead of hosting images yourself

---

## 🌐 Publishing an update

```bash
git add .
git commit -m "Day 5 - Florence"
git push
```

Vercel picks it up automatically and deploys in ~30 seconds.

**From your phone:** use the GitHub mobile app to create/edit files directly, or use Working Copy (iOS) for a full git client.

---

## 🎨 Customization

- **Blog name & subtitle:** edit `src/layouts/BaseLayout.astro`, find the `blogName` variable at the top
- **Colors:** edit the `:root` CSS variables in the same file
- **Your own domain:** add it in the Vercel dashboard under Project Settings → Domains
