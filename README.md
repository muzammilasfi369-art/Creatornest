# 🪺 CreatorNest

An all-in-one platform for content creators — schedule posts, write AI captions, generate hashtags, design thumbnails, and track analytics across all platforms.

---

## 🚀 How to Set Up & Deploy (Step by Step)

### Step 1 — Install Node.js
Download and install Node.js from: https://nodejs.org  
(Choose the LTS version)

---

### Step 2 — Download This Code
1. Create a GitHub account at https://github.com if you don't have one
2. Create a new repository called `creatornest`
3. Upload all these files to that repository

---

### Step 3 — Install Dependencies
Open Terminal (Mac) or Command Prompt (Windows), navigate to the project folder and run:

```bash
npm install
```

---

### Step 4 — Run Locally (to test on your computer)
```bash
npm run dev
```
Then open your browser and go to: **http://localhost:3000**

---

### Step 5 — Deploy Live to Vercel (FREE)
1. Go to https://vercel.com and sign up with your GitHub account
2. Click **"Add New Project"**
3. Select your `creatornest` GitHub repository
4. Click **"Deploy"** — Vercel handles everything automatically!
5. Your site will be live at: `https://creatornest.vercel.app` (or your custom domain)

---

### Step 6 — Add AI Functionality (Optional — for AI Caption Writer & Hashtag Generator)
The AI tools use the Anthropic Claude API. To enable them:

1. Go to https://console.anthropic.com and create an account
2. Get your API key
3. In Vercel, go to your project → Settings → Environment Variables
4. Add: `NEXT_PUBLIC_ANTHROPIC_API_KEY` = your key

> ⚠️ Note: The free tier of Anthropic API gives you enough credits to test. AI tools will cost a small amount per use at scale.

---

## 📁 File Structure

```
creatornest/
├── pages/
│   ├── index.js              ← Homepage (Landing Page)
│   ├── 404.js                ← Not Found page
│   ├── login/index.js        ← Login page
│   ├── signup/index.js       ← Signup page
│   ├── pricing/index.js      ← Pricing page
│   ├── tools/
│   │   ├── index.js          ← All Tools page
│   │   ├── caption-writer.js ← AI Caption Writer (uses Claude API)
│   │   ├── hashtag-generator.js ← Hashtag Generator (uses Claude API)
│   │   ├── thumbnail-maker.js   ← Thumbnail Maker
│   │   └── link-in-bio.js       ← Link in Bio Builder
│   ├── scheduler/index.js    ← Social Media Scheduler
│   └── analytics/index.js    ← Analytics Dashboard
├── components/
│   ├── Navbar.js             ← Navigation bar
│   └── Footer.js             ← Footer
├── styles/
│   └── globals.css           ← Global styles
├── package.json
├── tailwind.config.js
├── postcss.config.js
└── next.config.js
```

---

## 🛠️ Pages Included

| Page | URL | Description |
|------|-----|-------------|
| Landing Page | `/` | Homepage with hero, features, pricing |
| All Tools | `/tools` | Overview of all creator tools |
| AI Caption Writer | `/tools/caption-writer` | AI-powered caption generator |
| Hashtag Generator | `/tools/hashtag-generator` | Smart hashtag finder |
| Thumbnail Maker | `/tools/thumbnail-maker` | YouTube thumbnail designer |
| Link in Bio | `/tools/link-in-bio` | Bio link page builder |
| Scheduler | `/scheduler` | Multi-platform post scheduler |
| Analytics | `/analytics` | Cross-platform analytics dashboard |
| Pricing | `/pricing` | Plans & FAQ |
| Login | `/login` | Sign in page |
| Sign Up | `/signup` | Registration page |

---

## 💰 Cost Summary

| Service | Cost |
|---------|------|
| GitHub | FREE |
| Vercel Hosting | FREE |
| Custom Domain (optional) | ~$12/year |
| Anthropic API (AI tools) | Pay per use (~$0.001 per caption) |

---

## 🔮 Future Features to Add
- Real user authentication (Supabase or Firebase — free tier available)
- Actual social media API connections (Meta API, YouTube API)
- Real-time analytics from connected accounts
- Full thumbnail drag-and-drop editor
- Email newsletter tool
- Mobile app (React Native)

---

Built with: Next.js · Tailwind CSS · Anthropic Claude API  
Hosted on: Vercel  
© 2025 CreatorNest
