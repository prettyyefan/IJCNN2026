
# 激活虚拟环境
.\venv\Scripts\activate 

# 上传github仓库步骤
# first
git init

git add memo.md

git commit -m "first commit code"

git branch -M main

git remote add origin https://github.com/prettyyefan/IJCNN2026.git

git pull origin main --allow-unrelated-histories

git add LICENSE

git commit -m "anonymize license"

git push -u origin main