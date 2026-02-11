# 1. Start from latest main
git checkout main
git pull origin main
# 2. Create your feature branch
git checkout -b feature-your-feature-name
# 3. Make changes, then stage files
git add <files-you-changed>
# 4. Commit with a clear message
git commit -m "Description of your changes"
# 5. Push to GitHub
git push origin feature-your-feature-name
# 6. Go to GitHub.com → Create Pull Request → Merge
