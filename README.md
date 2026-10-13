# AR Heritage — Landing Page & Deployment Package

This standalone folder contains the complete, self-contained landing page website for **AR Heritage** (`Sulu Heritage Tech`).

All asset paths are **100% relative** (`./assets/...` and `./downloads/...`), meaning this entire folder can be moved anywhere, uploaded to any new GitHub repository, or deployed to any hosting platform with **zero configuration or build steps**.

---

## 📁 Folder Structure

```
landing_page/
├── index.html                           # Single-page high-converting product landing page
├── assets/                              # App screenshots, architecture charts & icons
│   ├── app_icon.png                     # Gold Pagoda startup logo & favicon
│   ├── scan_interface.jpeg              # Live camera scan interface with gold reticle
│   ├── detail_nyatapola.jpeg            # Nyatapola Temple historical record & details
│   ├── detail_facts.jpeg                # Key architectural facts & photo gallery
│   ├── home_screen.jpeg                 # Editorial Heritage of Nepal home feed
│   ├── gallery_viewer.jpeg              # Interactive full-screen gallery viewer
│   ├── training_history.png             # Figure 4.1: Distillation curves over 64 epochs
│   ├── confusion_matrix.png             # Figure 4.2: 3-class confusion matrix
│   └── component_architecture.png       # Figure 3.7: 4-layer system component diagram
├── downloads/
│   └── ar_heritage_v1.0_beta.apk        # Production-signed Android APK (80.5 MB)
└── README.md                            # Deployment documentation
```

---

## 🚀 Instant Deployment Options

### Option 1: Deploy as a New GitHub Repository (GitHub Pages)

1. Create a new repository on GitHub (e.g., `ar-heritage-landing` or `ar-heritage-web`).
2. Initialize and push this `landing_page` directory:
   ```bash
   cd landing_page
   git init
   git add .
   git commit -m "feat: initial commit of AR Heritage landing page"
   git branch -M main
   git remote add origin https://github.com/<your-username>/ar-heritage-landing.git
   git push -u origin main
   ```
3. Go to **Repository Settings &rarr; Pages**:
   - Under **Build and deployment**, select **Source**: `Deploy from a branch`.
   - Branch: `main` / Folder: `/ (root)`.
   - Click **Save**.
4. Your website will be live at `https://<your-username>.github.io/ar-heritage-landing/` in seconds!

---

### Option 2: Deploy within your Existing Repository (`/docs` folder)

If you prefer to keep the landing page inside your existing `ar_heritage` repository:
1. Copy the contents of this folder into a `docs/` folder in the root of your repo.
2. In GitHub repository **Settings &rarr; Pages**, choose **Source**: `Deploy from a branch` &rarr; Branch `main` &rarr; Folder `/docs`.

---

### Option 3: Deploy on Vercel (1-Click Drag & Drop)

1. Open [vercel.com](https://vercel.com).
2. Click **Add New &rarr; Project**.
3. Import your GitHub repository or simply drag and drop the `landing_page` folder.
4. **Framework Preset**: `Other` (Static HTML).
5. Click **Deploy**.

---

### Option 4: Deploy on Netlify

1. Open [app.netlify.com](https://app.netlify.com/drop).
2. Drag and drop the `landing_page` folder onto the browser window.
3. Your site is deployed instantly on a `.netlify.app` subdomain with global SSL CDN.

---

## 💻 Local Testing & Preview

You can open `index.html` directly in any web browser, or serve it locally:

```bash
# Python
python -m http.server 3000

# Node.js
npx serve .
```

Navigate to `http://localhost:3000` to view the page.
