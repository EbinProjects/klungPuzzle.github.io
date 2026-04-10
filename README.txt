git commadads

git init -Initialize your local folder

git remote add origin https://github.com/EbinProjects/klungPuzzle.github.io.git -Connect to GitHub (The "Remote" link)

. Upload your files- git add .

Prepare the files: -git commit -m "Connecting local folder to GitHub"

Send it to the web:-git branch -M main
git push -u origin main

Pull the changes from GitHub:-git pull origin main --rebase

f you get a "Refusing to merge unrelated histories" error-git pull origin main --allow-unrelated-histories


Fix — Disable Jekyll (Most Important Step)

Do this:

Open your repo:

klungPuzzle.github.io

Click:

Add file → Create new file
File name:
.nojekyll

⚠️ Important:

No extension
Exactly .nojekyll
Starts with a dot
Leave file empty
Click:
Commit changes
Why This Fix Works

GitHub Pages is trying to process:

assets/css/style.scss

But your project only has:

index.html
index.css
assets/images/

Adding .nojekyll tells GitHub:

Don't process SCSS
Don't use Jekyll
Just serve files as-is

This fixes most GitHub Pages failures.
