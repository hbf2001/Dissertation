```bash

# Pull latest changes from GitHub
!git pull origin master

### 1. Mount Google Drive
from google.colab import drive
drive.mount('/content/drive')

### 2. Go to your project folder
%cd /content/drive/MyDrive/Dissertation

### 3. Trust GitHub SSH host (only needed once per Colab session)
!mkdir -p ~/.ssh
!ssh-keyscan github.com >> ~/.ssh/known_hosts

### 4. Stage, commit, and push changes to GitHub
!git add .
!git commit -m "Your commit message"
!git push origin master
