# Git Project 2: Fork the facilitator's repo and add your files

Windows Command Prompt. Type one line at a time and press Enter.
Replace anything in `<ANGLE-BRACKETS>` with your own value.

## Do once first

```cmd
git --version
git config --global user.name "<YOUR-NAME>"
git config --global user.email "<YOUR-EMAIL>"
```

## 1. Fork the facilitator's repo (in browser)

Open the facilitator's repo on GitHub and click **Fork**. You now have your
own copy. Copy its URL from the green **Code** button.

## 2. Clone your fork and link the original

```cmd
cd %USERPROFILE%\Documents
git clone <YOUR-FORK-URL>
cd <REPO-NAME>
git remote add upstream <FACILITATOR-REPO-URL>
```

## 3. Make a branch, then your practice files

```cmd
git checkout -b practice-<YOURNAME>
mkdir <YOURNAME>
echo My answers > <YOURNAME>\practice1.txt
```

## 4. Stage, commit and push to your fork

```cmd
git status
git add .
git commit -m "Add practice files by <YOURNAME>"
git push -u origin practice-<YOURNAME>
```

## 5. Send your files to the facilitator (in browser)

Open your fork on GitHub, click **Compare & pull request**, then
**Create pull request**. Once the facilitator merges it, your files appear
in their repo.

## Tips

- **Lost?** Run `git status`
- **First push:** sign in to GitHub in the window that opens
- **Push rejected?** Run `git pull origin main`, then push again
