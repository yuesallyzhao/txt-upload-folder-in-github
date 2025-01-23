# txt-upload-folder-in-github
# how to upload a project folder to github repository by git command
# Download git.exe by https://git-scm.com/
# Open cmd and type, to ensure git is installed
git --version
# Go to your path of project folder, "cd\" is to go the root directory, "E:" is to your destination dir, "cd <path of your project folder>.
##### start to code #####
git init
# To add all files in your folder
git add . 
git commit -m "Initial commit"
# Add the github repository as the remote origin
git remote add origin https://github.com/your-username/your-repository-name.git
# Push the code to the main branch of your github
git branch -M main
git push -u origin main
# If you get an error like non-fast-forward, means remote repostory already has commits. Resolve:
git push -u origin main --force
