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

### *Github security token for HTTPS authentication:*

in github save a token under: **Settings => Developer settings => Personal access tokens => select all scopes => generate token**
**git config --global credential.helper cache:** Save pw in cache 

### *Markdown:*
Editor and viewer: [here](https://dillinger.io/) 
Markdown cheat sheet: [here](https://cheatography.com/lucbpz/cheat-sheets/the-ultimate-markdown/) 

### *Html & css links:*
- Automatic Scaling text: [https://type-scale.com/](https://type-scale.com/) 
- Templates: [https://dribbble.com/](https://dribbble.com/)
- Icons: [https://fontawesome.com/](https://fontawesome.com/) 
- Special text Fonts: [https://www.cdnfonts.com/](https://www.cdnfonts.com/) 
- Bootstrap cheat sheet: [https://bootstrap-cheatsheet.themeselection.com/](https://bootstrap-cheatsheet.themeselection.com/)
- Share maps with: [https://www.google.com/maps/about/mymaps/](https://www.google.com/maps/about/mymaps/)
- Free images: [https://unsplash.com/](https://unsplash.com/)

### *Css responsive code:*
*Key example:* 
```
@media only screen and (max-width: 480px){
.container h1{
    	Font-size: 50%;
    }
}
````
##### *Sizes for responsiveness*:
- **320px—480px**: Mobile devices
- **481px—768px**: iPads, Tablets
- **769px—1024px**: Small screens, laptops
- **1025px—1200px**: Desktops, large screens
- **1201px and more**: Extra large screens, TV

### *CSS frameworks*
 - Tailwind css.
 - Bootstrap [docs](https://getbootstrap.com/docs/5.2/getting-started/introduction/)
 - Bootstrap [cheat sheet](https://bootstrap-cheatsheet.themeselection.com/)
 - Bootstrap [crashcourse](https://youtu.be/4sosXZsdy-s)


### *Useful shortcuts and settings in VSC:*
- **mkdir ‘folder’ cd to the ‘folder’ ‘code .’:** opens VSC in the selected folder
- **Ctrl + ‘,’ :** goes to settings
- **In settings type “Relative path ” and choose for ‘/’:** Uses forward slash(/) instead of backslash (\) as relative path separator when copy and pasting a path. 
- **ctrl+k + ctrl+c / ctrl+u:** Comment and uncomment
- **Alt+click:** Several cursors
- **Ctrl + d:** Selects equal words and adds a cursor at it
- **shift + alt + down:** Copy Paste line down 
- **alt+up/down:** Move Line up/down 
- **select the word and ctrl+shift+f:** Search for a word in the project
- **ALT+SHIFT + ’F’:** format code in VSC.
- **Compare 2 files:** 
 Select 1st file, right click “select for compare”.
 Select 2nd file, right click “compare with selected”
 
 ### *Node-js*
 - npm: node packet manager
 - nvm: node version manager
 - totorial: https://www.youtube.com/watch?v=TlB_eWDSMt4
 
  ### *Backend*
  - create new project. cd new project
  - npm init
  - npm i express mangoose
  - npm i --save-dev dotenv nodemon
  - in packages add: 
  "scripts": {
    "devStart":"nodemon server.js" 
  },
  - you will need to start the script with npm run devStart. It will restart the server each time you save.
  - touch server.js, .env and .gitignore in root
  - ignore .env node_modules (add it in .gitignore)
  - rest client app extension on VSC to test API's
  
    - for later: Quick REST API Creation using Node-Restful Library.
    https://hostadvice.com/how-to/how-to-create-rest-api-with-node-express-and-mongoose/#paragraph4
