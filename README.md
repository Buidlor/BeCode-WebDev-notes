
### *Linux Ubuntu*
- Install linux ubuntu on wsl (ubuntu command line in windows): [Manual here](https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#3-download-ubuntu )
*or*
- Install ubuntu on Virtualbox: [Manual here](https://www.geeksforgeeks.org/how-to-install-ubuntu-on-virtualbox/)
*or*
- Install ubuntu Dual Boot: [Manual here](https://www.freecodecamp.org/news/how-to-dual-boot-windows-10-and-ubuntu-linux-dual-booting-tutorial/)

### *Github commands:*
- **Git init**: inits your folder
- **Git add .**: stage all changes
- **Git commit -m “ text”**: commit staged changes.
- **git commit --amend --no-edit** : amend staged changes to the last commit
- **Git remote add origin https://github.com/Buidlor/example:** github origin
- **git remote get-url origin** : View push origin:
- **git remote set-url origin https://git-repo/new-repository.git**: Change push origin:  
- **git push --set-upstream origin master:** Push code to github
- **Git pull:** update your local code by pulling out of github
- **git checkout -b “name_of_your_new_branch”:** Create your own branche: 
- **git checkout “existing branch”:** switch to existing branch.
- **git branch:** see what branch your in
- **git branch --delete <branch name>:** delete a branch
- **git status:** view status
- **git log:** view log
- **git merge –abort:** abort the merging process
- **git status:** view status 
- **Git log –oneline –graph:** Logs in graph format
- View all repos included shared ones: Settings -> Repositories

### *Github Push, pull and clone with SSH Authentication:*
- **ssh-keygen -t ed25519 -C "your_email@example.com"**
- **eval "$(ssh-agent -s)"**
- **ssh-add ~/.ssh/id_ed25519**
- **Copy the key from the generated file and paste it in your github website under settings => SSH key**
- Connect ssh to github: **ssh -T git@github.com**

### *Hithub security token for HTTPS authentication:*

in github save a token under: **Settings => Developer settings => Personal access tokens => select all scopes => generate token**
**git config --global credential.helper cache:** Save pw in cache 

### *Markdown:*
Editor and viewer: [here](https://dillinger.io/) 
Markdown cheat sheet: [here](https://cheatography.com/lucbpz/cheat-sheets/the-ultimate-markdown/) 

### *Html & css links:*
- Automatic Scaling text: https://type-scale.com/ 
- Templates: https://dribbble.com/
- Icons: https://fontawesome.com/ 
- Special text Fonts: https://www.cdnfonts.com/ 

### *Css responsive code:*
*Key example:* 
```
@media only screen and (max-width: 480px){
.container h1{
    	Font-size: 50%;
    }
}
````

##### *Sizes*:
- **320px—480px**: Mobile devices
- **481px—768px**: iPads, Tablets
- **769px—1024px**: Small screens, laptops
- **1025px—1200px**: Desktops, large screens
- **1201px and more**: Extra large screens, TV
