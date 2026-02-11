6.1 Switch to main and pull latest changes
Always start by making sure you have the latest version of the code:

git checkout main
git pull origin main

6.2 Create a new branch for your work
Create a descriptive branch name that reflects what you’re working on:
git checkout -b feature-changed-whatever

Examples of good branch names:
feature-add-claw-config
fix-claw-bug
update-readme-instructions

6.3 Make your changes and stage them
After editing your files, add the specific files you changed:
git add claw.cpp
git add main.cpp utils.h
Or to add all changed files at once:
git add .

6.4 Commit your changes
Write a clear commit message describing what you did:
git commit -m "Added claw machine dispensing logic"

6.5 Push your branch to GitHub
Push your branch to the remote repository:
git push origin feature-changed-whatever