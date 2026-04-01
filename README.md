# Heaven Operations Global — Deployment Guide

## What's in this folder

```
hog-site/
├── index.html                  ← Your main website
├── netlify.toml                ← Netlify configuration
├── admin/
│   ├── index.html              ← CMS login page (yoursite.netlify.app/admin)
│   └── config.yml              ← CMS fields & collections
└── content/
    ├── settings/
    │   ├── general.json        ← Site name, tagline
    │   └── about.json          ← About page text, mission, values
    ├── team/                   ← One JSON file per team member
    └── materials/              ← One JSON file per material
```

---

## Step-by-Step: Go Live in 20 Minutes

### Step 1 — Create a GitHub account
1. Go to https://github.com and sign up (free)
2. Click **"New repository"**
3. Name it: `heaven-operations-global`
4. Set it to **Public**
5. Click **"Create repository"**

### Step 2 — Upload your files
1. On your new repository page, click **"uploading an existing file"**
2. Drag the entire `hog-site` folder contents into the upload area
   (upload ALL files, keeping the folder structure intact)
3. Click **"Commit changes"**

### Step 3 — Create a Netlify account
1. Go to https://netlify.com and sign up with your GitHub account
2. Click **"Add new site"** → **"Import an existing project"**
3. Choose **GitHub** → select your `heaven-operations-global` repo
4. Leave all build settings as default
5. Click **"Deploy site"**
6. Your site will be live at a URL like: `amazing-name-123.netlify.app`
   (You can rename this in Site Settings → Domain)

### Step 4 — Enable the CMS login
1. In Netlify, go to **Site configuration → Identity**
2. Click **"Enable Identity"**
3. Under **Registration**, choose **"Invite only"** (so only your team can join)
4. Scroll to **Git Gateway** → click **"Enable Git Gateway"**

### Step 5 — Invite your team
1. Still in the Identity tab, click **"Invite users"**
2. Enter each team member's email address (up to 5 people)
3. They'll receive an email to set their password

### Step 6 — Log in to your CMS
1. Go to: `yoursite.netlify.app/admin`
2. Log in with your email
3. You'll see a dashboard to edit everything!

---

## What your team can edit in the CMS

| Section | What you can change |
|---|---|
| **Site Settings → General** | Site name, tagline |
| **Site Settings → About Us** | Intro paragraph, mission text, values |
| **Team Members** | Names, roles, initials, order — add/remove people |
| **Materials** | Add new books/modules/sermons, edit descriptions, add links |

## Adding a new material via CMS
1. Log in at `/admin`
2. Click **"Materials"** → **"New Material"**
3. Fill in: Title, Author, Category, Type, Description, Link
4. Click **"Publish"**
5. Site updates automatically within 30 seconds ✓

---

## Need help?
- Netlify docs: https://docs.netlify.com
- Decap CMS docs: https://decapcms.org/docs
