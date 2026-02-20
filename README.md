# Blog

Ultra minimal dark blog. Hugo + GitHub Pages.

## Setup

```bash
# 1. Install Hugo
sudo apt install hugo
# ou: snap install hugo

# 2. Clone ce repo
git clone https://github.com/TONUSERNAME/TONUSERNAME.github.io.git
cd TONUSERNAME.github.io

# 3. Preview local
hugo server -D

# 4. Nouveau post
hugo new posts/mon-article.md

# 5. Push → deploy automatique via GitHub Actions
git add -A && git commit -m "new post" && git push
```

## Structure

```
content/posts/    ← tes articles en markdown
themes/void/      ← le thème (ne touche à rien sauf css/style.css)
hugo.yaml         ← config
```
