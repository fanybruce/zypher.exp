# Zypher Application & Privacy Policy Portal

Official centralized developer portal and privacy policy repository for **Zypher** mobile applications. Hosted on GitHub Pages at:

🌐 **[https://fanybruce.github.io/zypher.exp/](https://fanybruce.github.io/zypher.exp/)**

---

## 📁 Repository Structure

```text
zypher.exp/
├── index.html                   # Central Hub Portal listing all Zypher applications
├── privacy/
│   ├── index.html               # General privacy directory listing all policies
│   └── puzzles/
│       └── index.html           # Dedicated Privacy Policy for Zypher Puzzles
├── puzzles/
│   └── privacy.html             # Direct alias permalink for store submissions
├── assets/
│   └── puzzles_icon.png         # Zypher Puzzles app icon
├── .nojekyll                    # Ensures clean static file serving on GitHub Pages
└── .github/
    └── workflows/
        └── pages.yml            # Automatic GitHub Pages deployment workflow
```

---

## 🔗 Live Application Privacy URLs

| Application | Package ID | Official Privacy Policy URL |
| :--- | :--- | :--- |
| **Zypher Puzzles** | `com.zypher.puzzlegame` | [https://fanybruce.github.io/zypher.exp/privacy/puzzles/](https://fanybruce.github.io/zypher.exp/privacy/puzzles/) *(or `.../puzzles/privacy.html`)* |

---

## 🚀 How to Add a New App in the Future

When releasing a new app under the Zypher publisher account:

1. **Create Policy Folder**:
   Create a new directory under `privacy/<app_name>/` (e.g. `privacy/greedysnake/index.html`).
2. **Copy the Template**:
   Copy `privacy/puzzles/index.html`, update the title, package ID (`com.zypher.<app_name>`), and specific feature permissions.
3. **Register on Main Portal**:
   Add a card for the new app in root `index.html` and a listing entry in `privacy/index.html`.
4. **Push to GitHub**:
   ```bash
   git add .
   git commit -m "feat: add privacy policy for <app_name>"
   git push origin main
   ```
   GitHub Pages will automatically deploy the update within seconds!
