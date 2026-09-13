# Zypher Application & Privacy Policy Portal

Official centralized developer portal and privacy policy repository for **Zypher** mobile applications. Hosted on GitHub Pages at:

🌐 **[https://fanybruce.github.io/zypher.exp/](https://fanybruce.github.io/zypher.exp/)**

---

## 📁 Repository Structure

Each application has its own dedicated, self-contained folder containing every document and asset required for store submission and user disclosure:

```text
zypher.exp/
├── index.html                   # Central Hub Portal listing all Zypher applications
├── privacy/
│   └── index.html               # General privacy directory listing all policies
├── puzzles/                     # Zypher Puzzles self-contained app folder
│   ├── index.html               # Privacy Policy
│   ├── privacy.html             # Store submission permalink
│   └── icon.png                 # App icon
├── game_2048/                   # 2048+ self-contained app folder
│   ├── index.html               # Privacy Policy
│   ├── privacy.html             # Store submission permalink
│   └── icon.png                 # App icon
├── .nojekyll                    # Ensures clean static file serving on GitHub Pages
└── .github/
    └── workflows/
        └── pages.yml            # Automatic GitHub Pages deployment workflow
```

---

## 🔗 Live Application Privacy URLs

| Application | Package ID | Official Privacy Policy URL | Direct Store Permalink |
| :--- | :--- | :--- | :--- |
| **Zypher Puzzles** | `com.zypher.puzzlegame` | [https://fanybruce.github.io/zypher.exp/puzzles/](https://fanybruce.github.io/zypher.exp/puzzles/) | `.../puzzles/privacy.html` |
| **2048+** | `com.zypher.game_2048` | [https://fanybruce.github.io/zypher.exp/game_2048/](https://fanybruce.github.io/zypher.exp/game_2048/) | `.../game_2048/privacy.html` |

---

## 🚀 How to Add a New App in the Future

When releasing a new app under the Zypher publisher account:

1. **Create Dedicated App Folder**:
   Create a new directory at the repository root: `<app_name>/` (e.g. `greedysnake/`).
2. **Add Required Application Docs & Assets**:
   Inside `<app_name>/`, add:
   - `icon.png`: High-resolution application icon.
   - `index.html`: Privacy policy based on the Zypher privacy template.
   - `privacy.html`: Alias copy of `index.html` for direct store URLs.
3. **Register on Main Portal**:
   Add an app card in root `index.html` and a listing row in `privacy/index.html`.
4. **Push to GitHub**:
   ```bash
   git add .
   git commit -m "feat: add privacy docs for <app_name>"
   git push origin main
   ```
   GitHub Pages will automatically deploy the update within seconds!
