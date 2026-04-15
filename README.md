# Oman eVisa Portal — Static Site

A pixel-perfect, single-file recreation of the **Oman eVisa "Track Your Application"** portal interface, built with plain HTML, CSS, and JavaScript. No build tools, no dependencies, no server required.

---

## 📁 Project Structure

```
evisa-portal/
├── index.html       ← Entire application (HTML + CSS + JS, self-contained)
├── netlify.toml     ← Netlify deployment configuration
└── README.md        ← This file
```

---

## 🚀 Deploy to Netlify (3 steps)

### Option A — Drag & Drop (fastest)
1. Go to [netlify.com](https://netlify.com) and log in
2. Drag the entire `evisa-portal` folder onto the Netlify dashboard
3. Your site is live instantly ✅

### Option B — GitHub → Netlify (recommended for updates)
1. Push this folder to a GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/evisa-portal.git
   git push -u origin main
   ```
2. Go to [app.netlify.com](https://app.netlify.com) → **Add new site** → **Import from Git**
3. Select your GitHub repo
4. Build settings (leave defaults — they are already set in `netlify.toml`):
   - **Build command:** *(leave empty)*
   - **Publish directory:** `.`
5. Click **Deploy site** ✅

Every future `git push` will automatically redeploy.

---

## ✏️ How to Edit Data

All personal data is plain HTML inside `index.html`. Search for these IDs:

| Field | Element ID |
|---|---|
| Visa Application Number | `visaAppNum` (input value) |
| Travel Document Number | `travelDocNum` (input value) |
| Visa Number | `d-visaNumber` |
| Given Name | `d-givenName` |
| Family Name | `d-familyName` |
| Gender | `d-gender` |
| Nationality | `d-nationality` |
| Travel Doc Expiry | `d-expiry` |
| Occupation | `d-occupation` |

---

## 🖥️ Run Locally

No server needed. Just open in a browser:
```bash
open index.html
# or double-click index.html in your file manager
```

---

## 🔧 Tech Stack

- Pure HTML5 / CSS3 / Vanilla JS
- [Font Awesome 6.4](https://fontawesome.com) (via CDN, icons only)
- No frameworks, no npm, no build step

---

## 📄 License

For internal/demo use only. Royal Oman Police and Oman eVisa branding belongs to their respective owners.
