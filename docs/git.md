# configuration
git config --global user.email "dgueudre@gmail.com"
git config --global user.name "Davy Gueudré"
git config --global color.ui true
git config --list

# courant
git status

# staging
git add <fileName>
git add "*.html"
git add --all (inclus les suppression)

# commit
git commit -a
git commit -a -m "test"

# log
git log -n 2
git log --oneline
git log -p readme.md

# diff
git diff

# checkout
git checkout 2483ed6
git checkout 2483ed6 index.html

# revert
git revert 2483ed6
git revert 2483ed6 index.html

# reset dangereux
git reset 2483ed6
git reset HEAD index.html
git reset -- index.htmlgit 
git reset HEAD^^^ (revient 3 crans en arrière)

git reset HEAD --soft (modif dans staging)
git reset HEAD --mixed (modif à stagger [défault])
git reset HEAD --hard (suppression des modifications)