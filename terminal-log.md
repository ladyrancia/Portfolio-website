# Terminal Log - Tasks 5.1 to 6.4

## Task 5.1: Terminal Navigation
```bash
pwd
ls
cd ~/Documents
cd ..
cd ~
```

## Task 5.1: Create Project Structure
```bash
mkdir -p my-project/src/{css,js,images} my-project/docs my-project/tests
touch my-project/README.md
```

## Task 5.2: File Operations
```bash
cd my-project
touch index.html
cat index.html
cp index.html backup.html
mv backup.html docs/
mv index.html home.html
rm home.html
cp -r src src-backup
mv src-backup archive
rm -r archive
cd ..
```

## Task 5.3: Useful Commands and Answers
```bash
find . -name "*.html"
grep "class" my-project/src/index.html
grep -r "button" ./my-project/src/
head -10 my-project/src/css/styles.css
tail -10 my-project/src/css/styles.css
wc my-project/src/index.html
wc -l my-project/src/css/styles.css
```

### Answers (command output)
- How many HTML files are in this project? `4`
- Which files contain the word "contact"?
  - `./my-project/src/index.html`
  - `./my-project/src/css/styles.css`
  - `./index.html`
  - `./styles.css`
- How many lines is the CSS file? `3`
- What were your last 10 terminal commands? not available in this non-interactive shell session (`history` has no persisted entries).

## Task 5.4: Shell Script Basics
Created and tested:
```bash
chmod +x new-project.sh
./new-project.sh my-awesome-app
```

## Task 6.1: Git Basics
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --list
git init
git status
git add .
git commit -m "Initial commit: portfolio structure"
git log --oneline
```

## Task 6.2: Branching & Merging
```bash
git branch
git branch feature/contact-form
git switch feature/contact-form
git switch -c feature/about-page
# edit about.html
git add about.html
git commit -m "feat: add about page"
git switch main
git merge feature/about-page
git branch -d feature/about-page
```

## Task 6.3: GitHub Remote Workflow
```bash
git remote add origin https://github.com/yourusername/iyf-s10-week-03-yourusername.git
git remote -v
git push -u origin main
git clone https://github.com/yourusername/iyf-s10-week-03-yourusername.git week03-clone
git pull origin main
```

## Task 6.4: Professional README
- Updated `README.md` with all required sections.
- Added `.gitignore` entries for dependencies, IDE folders, OS files, and temp files.
