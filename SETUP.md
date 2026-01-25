# 🚀 Quick Setup

## Deploy to GitHub Pages

### 1. Create Repository
1. Go to https://github.com/new
2. Repository name: `MFT_Exam_Master`
3. Public repository
4. Don't initialize with README
5. Click "Create repository"

### 2. Push Your Code
```bash
cd /path/to/MFT_Exam_Master

git init
git add .
git commit -m "Initial commit: MFT Exam Master"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/MFT_Exam_Master.git
git push -u origin main
```

### 3. Enable GitHub Pages
1. Go to repository Settings
2. Click "Pages" in sidebar
3. Source: Deploy from branch
4. Branch: `main`
5. Folder: `/ (root)`
6. Click Save

### 4. Access Your Site
Wait 2-3 minutes, then visit:
`https://YOUR-USERNAME.github.io/MFT_Exam_Master/`

---

## Local Development

To run locally:
1. Double-click `index.html`
2. Opens in your default browser
3. Works completely offline!

---

## Updating Questions

To add more questions:
1. Edit files in `questions/` folder
2. Follow the JSON format
3. Commit and push:
```bash
git add questions/
git commit -m "Add more questions"
git push
```

Site updates automatically in 1-2 minutes!

---

## Need Help?

- Check the [README](README.md) for full documentation
- Open an issue on GitHub
- Review keyboard shortcuts: Press `?` in the app
