#Lab 8: Read Me on How to Create Repo
I created my repo by first copying it to my local linux system using terminal. I then identified myself to Git using my name and my github username in the terminal. I then set up the SSH keys so that my computer and GitHub communicated efficiently without having to type a passwrod everytime to allow access. I added my new key and also displayed my public key. I added the key to my Github account in the section in settings labeled "SSH and GPG Keys." I ensured my clone worked and played around with a couple of commands to better learn the environment and to get comfortable with the code used. 

This is a summary of the code used to make this work:
# Configure Git
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

# Create SSH key
ssh-keygen -t ed25519 -C "you@example.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
cat ~/.ssh/id_ed25519.pub

# Clone, edit, and sync
git clone git@github.com:username/repo.git
cd repo
pico README.md
git add README.md
git commit -m "First edit"
git push
git pull

Remember, whenever you do a code related project, make sure to upload it to the repo so that you have a secondary spot storing the code. 
