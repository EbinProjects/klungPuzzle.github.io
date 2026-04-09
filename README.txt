git commadads

git init -Initialize your local folder

git remote add origin https://github.com/EbinProjects/klungPuzzle.github.io.git -Connect to GitHub (The "Remote" link)

. Upload your files- git add .

Prepare the files: -git commit -m "Connecting local folder to GitHub"

Send it to the web:-git branch -M main
git push -u origin main

Pull the changes from GitHub:-git pull origin main --rebase

f you get a "Refusing to merge unrelated histories" error-git pull origin main --allow-unrelated-histories