---
title: "Building This Blog: Why I Chose Hugo + Cloudflare Pages (and How You Can Too)"
date: 2025-04-12
tags: ["hugo", "cloudflare-pages", "blogging", "static-sites", "neovim", "git"]
draft: false
image: "https://images.unsplash.com/photo-1587620962725-abab7fe55159?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=80"
---

![Hugo Static Site Generator](https://raw.githubusercontent.com/gohugoio/hugoDocs/master/static/images/hugo-logo-wide.svg)
*Image: Hugo’s fast and flexible static site generator*

When I set out to create this blog, I wanted something clean, fast, and developer-friendly — no bloated CMS, no heavy backend. After exploring a few options, I settled on:

- 🏗 **Hugo** for static site generation  
- ☁️ **Cloudflare Pages** for hosting  
- 🧠 **Neovim** for writing posts in Markdown  
- 🐙 **GitHub** for version control and deployments

Here’s why I picked this combo — and how you can set it up too.

---

## 🧱 Why Hugo?

I chose Hugo because it’s a perfect balance of simplicity and performance:

- ⚡ **Super fast builds** (even with lots of posts)
- 🧩 **Tons of themes**, easily customizable
- ✍️ **Markdown-based content**, no weird editors or databases
- 💡 **Great for version control** — your entire site is just files in a repo

---

## ☁️ Why Cloudflare Pages?

Cloudflare Pages made deployment ridiculously easy. I was up and running in minutes.

- 🔗 **Direct GitHub integration**  
- 🚀 **Automatic deployment** on push  
- 🔒 **Free HTTPS** and **global CDN**  
- 📊 **Built-in analytics + performance**

It’s free, fast, and just works.

---

## 💻 My Actual Workflow

- I write blog posts using **Neovim** in Markdown (with a nice TUI + plugins).
- I push changes to **GitHub**.
- Cloudflare Pages **auto-deploys** the site.
- I can preview locally using `hugo server`.

Here’s what it looks like:

![Neovim Markdown Preview](https://user-images.githubusercontent.com/7425265/191087341-44a6b3e1-f683-4e99-a1aa-055cf20478fd.png)
*Image: Neovim in action with Markdown and Hugo preview*

---

## 🛠️ How to Set Up a Blog Like Mine

Here’s a quick-start guide if you want to build your own Hugo blog, just like this:

### 1. Install Hugo

```bash
brew install hugo  # macOS
# or for Linux
sudo apt install hugo
```

Or [download it from the official site](https://gohugo.io/getting-started/installing/).

---

### 2. Create Your Site

```bash
hugo new site myblog
cd myblog
git init
```

Pick a theme from [themes.gohugo.io](https://themes.gohugo.io) and follow its setup instructions.

---

### 3. Add Your First Post

```bash
hugo new posts/my-first-post.md
```

Edit it using **Neovim** or your favorite editor. I use a TUI like `telescope.nvim`, `markdown-preview.nvim`, and Git integration.

---

### 4. Version Control with GitHub

```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git add .
git commit -m "Initial commit"
git push -u origin main
```

---

### 5. Deploy with Cloudflare Pages

- Go to [pages.cloudflare.com](https://pages.cloudflare.com/)
- Click **"Create a Project"**
- Connect to your GitHub repo
- Use these settings:

```
Framework: Hugo
Build command: hugo
Publish directory: public
```

That’s it. Cloudflare will handle builds and deploys every time you push.

---

## Final Thoughts

If you want a **blazing-fast blog**, full control with Markdown, and zero hosting headaches — this stack is 🔥.

Let me know if you want me to break down any step further or dive into my Neovim setup (I’ve tuned it pretty well for blogging!).

---

Cheers,  
**Najib**
```

---

Let me know if you want me to:
- Generate a custom banner image with your name/logo on it
- Show how to make the featured image show up in social previews (Open Graph / Twitter cards)
- Turn your Neovim setup into a full “My Dev Writing Setup” post (which people love)

Want to do that next?

