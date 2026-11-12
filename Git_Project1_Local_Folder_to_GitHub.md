# Git Project 1: Start from scratch — local folder to GitHub

Windows Command Prompt. Type one line at a time and press Enter.
Replace anything in `<ANGLE-BRACKETS>` with your own value.

## Do once first

```cmd
git --version
git config --global user.name "<YOUR-NAME>"
git config --global user.email "<YOUR-EMAIL>"
```

## 1. Create the folder and files

```cmd
cd %USERPROFILE%\Documents
mkdir project1 && cd project1
echo # Project 1 > README.md
echo print("Hello Git") > hello.py
```

## 2. Start Git and save a first commit

```cmd
git init
git status
git add .
git commit -m "Initial commit"
```

## 3. Create an empty repo on GitHub (in browser)

On github.com choose **New repository** and name it `project1`.
Do **not** tick "Add a README". Copy the repo URL from the next page.

## 4. Connect the folder and push

```cmd
git branch -M main
git remote add origin <YOUR-REPO-URL>
git push -u origin main
```

## 5. Repeat after every change

```cmd
git add .
git commit -m "<WHAT-YOU-CHANGED>"
git push
```

## Tips

- **Lost?** Run `git status`
- **First push:** sign in to GitHub in the window that opens
- **Push rejected?** Run `git pull origin main`, then push again
