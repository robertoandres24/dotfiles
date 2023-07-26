```sh
# Sync SymLinks in local
stow --adopt -nvt ~ *
# Clone the repo, and delete this README.md file
# Inside the cloned dotfiles folder, execute:
stow -nvt ~ *
# Check the ouptut, and execute the same coomand without the -n flag

#Syncing New Changes:
#Whenever you make changes to your dotfiles, update them in the respective application's subdirectory within your dotfiles directory.
#To sync the changes with stow, navigate to the dotfiles directory and run:
stow -R <application>

# commit and push to remote repo
git add .
git commit -m "Update dotfiles: <describe changes>"
git push origin master
```
