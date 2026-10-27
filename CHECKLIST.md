# 🚀 Go-Live Checklist & Repository Guide
**Repository:** `codedbymuneeb/codedbymuneeb`  
**Reference Match:** [Sushmitadasari](https://github.com/Sushmitadasari) (Pixel-Level Motion & Polish)

---

## 📌 Placeholders to Replace in `README.md`

| Item | Placeholder | Where to Replace | What to Enter |
| :--- | :--- | :--- | :--- |
| **LinkedIn** | `YOUR-LINKEDIN-USERNAME` | Top badges (Line 8) & Connect badges (Line 59) | Your LinkedIn handle (e.g. `mian-muneeb`) |
| **Email** | `YOUR-EMAIL@gmail.com` | Top badges (Line 9) & Connect badges (Line 58) | Your email (e.g. `mianmuneeb3322@gmail.com`) |
| **Project 1** | `SPEECH-EMOTION-REPO` | Selected Work Section (Lines 20, 24) | Exact repo name for Speech Emotion Recognition |
| **Project 2** | `LLM-CHATBOT-REPO` | Selected Work Section (Lines 28, 32) | Exact repo name for LLM Chatbot |
| **Project 3** | `COMPUTER-VISION-REPO` | Selected Work Section (Lines 36, 40) | Exact repo name for Computer Vision |
| **Project 4** | `US-ACCIDENTS-REPO` | Selected Work Section (Lines 44, 48) | Exact repo name for US Accidents Analysis |

---

## 🐍 Contribution Snake Setup & Troubleshooting

The contribution snake uses `.github/workflows/snake.yml` to automatically generate the contribution graph every midnight UTC and on manual trigger (`workflow_dispatch`).

### 1. Enable GitHub Actions Permissions
1. Navigate to your repository on GitHub: `https://github.com/codedbymuneeb/codedbymuneeb`
2. Go to **Settings** → **Actions** → **General**.
3. Scroll down to **Workflow permissions**.
4. Select **Read and write permissions**.
5. Check the box **Allow GitHub Actions to approve pull request requests** and click **Save**.

### 2. Run the Workflow Manually (First Time)
1. Go to the **Actions** tab on GitHub: `https://github.com/codedbymuneeb/codedbymuneeb/actions`.
2. Click on the **Generate Contribution Snake** workflow on the left sidebar.
3. Click the **Run workflow** dropdown button on the right and select the `main` branch.
4. Click the green **Run workflow** button.
5. Once complete (green checkmark, ~30-45 seconds), it will automatically create and publish to the `output` branch.

### 3. Graceful Fallback (Why It Never Breaks Now)
- The README uses a `<picture>` element linking to `output/contribution-snake.svg` with a local fallback to `assets/contribution-snake.svg`.
- Even before the workflow runs or if GitHub camo proxy is caching, the README will **never show a broken image**—it seamlessly renders the custom crimson animated contribution snake directly from `assets/`!

---

## 📦 Pushing Changes to GitHub

Run these commands in PowerShell or your terminal:

```powershell
# 1. Stage all changes
git add README.md CHECKLIST.md .github/ assets/

# 2. Commit the changes
git commit -m "feat: complete pixel-level motion match with reference profile, animated SVGs, and snake fallback"

# 3. Push to GitHub
git push origin main
```

*(Note: If your local git credentials lack the `workflow` scope for pushing `.github/workflows/snake.yml`, you can either push with a Personal Access Token (PAT) having `workflow` scope, or add/edit `.github/workflows/snake.yml` directly on GitHub web via **Add file** -> **Create new file**).*
