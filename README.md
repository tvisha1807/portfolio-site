# Tvisha Pandey — Portfolio

Personal portfolio site for Tvisha Pandey, UX Designer.

**Live site:** [tvishapandey.me](https://tvishapandey.me)  
**Staging:** Vercel preview URL (auto-generated per branch)

## Stack

- [Astro 6](https://astro.build) — static site framework
- [Tailwind CSS v4](https://tailwindcss.com) — utility styling
- [MDX](https://mdxjs.com) — case studies as Markdown
- [React](https://react.dev) — interactive islands
- [Vercel](https://vercel.com) — hosting & CI/CD
- [Porkbun](https://porkbun.com) — domain registrar

## Local development

```bash
pnpm install
pnpm dev          # http://localhost:4321
```

## Adding a project

Create a new `.mdx` file in `src/content/projects/`:

```md
---
title: "Project Name"
description: "One-sentence description"
tags: ["UX Research", "Interaction Design"]
coverImage: "/images/projects/my-project.jpg"
year: 2025
role: "Lead UX Designer"
featured: true
order: 2
---

## Overview
...
```

The page will be available at `/work/<filename-without-extension>`.

## Deploy

Every push to `main` auto-deploys via Vercel. Pull request branches get a unique preview URL.

## Contact form

The contact form uses [Web3Forms](https://web3forms.com) (free, 100 submissions/mo).  
Replace `YOUR_WEB3FORMS_KEY` in `src/pages/contact.astro` with the key from your Web3Forms account.
