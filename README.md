### *Linux Ubuntu*
- Install linux ubuntu on wsl (ubuntu command line in windows): [Manual here](https://ubuntu.com/tutorials/install-ubuntu-on-wsl2-on-windows-10#3-download-ubuntu )
*or*
- Install ubuntu on Virtualbox: [Manual here](https://www.geeksforgeeks.org/how-to-install-ubuntu-on-virtualbox/)
*or*
- Install ubuntu Dual Boot: [Manual here](https://www.freecodecamp.org/news/how-to-dual-boot-windows-10-and-ubuntu-linux-dual-booting-tutorial/)

### *Github commands:*
- **`Git init`**: inits your folder
- **`Git add .`**: stage all changes
- **`Git commit -m “ text”`**: commit staged changes.
- **`git commit --amend --no-edit`** : amend staged changes to the last commit
- **`Git remote add origin https://github.com/Buidlor/example:`** github origin
- **`git remote get-url origin`** : View push origin:
- **`git remote set-url origin https://git-repo/new-repository.git`**: Change push origin:  
- **`git push --set-upstream origin master:`** Push code to github
- **`Git pull`** : update your local code by pulling out of github
- **`git checkout -b “name_of_your_new_branch”`:** Create your own branche: 
- **`git checkout “existing branch”:`** switch to existing branch.
- **`git branch`:** see what branch your in
- **`git branch --delete <branch name>`:** delete a branch
- **`git status`:** view status
- **`git log`:** view log
- **`git merge –abort`:** abort the merging process
- **`git status`:** view status 
- **`Git log –oneline –graph`:** Logs in graph format
- View all repos included shared ones: **Settings -> Repositories**

### *Github Push, pull and clone with SSH Authentication:*
- **`ssh-keygen -t ed25519 -C "your_email@example.com"`**
- **`eval "$(ssh-agent -s)"`**
- **`ssh-add ~/.ssh/id_ed25519`**
- **Copy the key from the generated file and paste it in your github website under settings => SSH key**
- Connect ssh to github: **`ssh -T git@github.com`**

### *Github security token for HTTPS authentication:*

- In github save a token under: **Settings => Developer settings => Personal access tokens => select all scopes => generate token**
- Save pw in cache: **`git config --global credential.helper cache`** 

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
 
 
# Backend
 ### *Node-js*
 - npm: node packet manager
 - nvm: node version manager
 - totorial: https://www.youtube.com/watch?v=TlB_eWDSMt4
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
  
    - for later: Quick REST API Creation using Node-Restful Library. [Tutorial]( https://hostadvice.com/how-to/how-to-create-rest-api-with-node-express-and-mongoose/#paragraph4)
    - Fullstack Authentication app [Tutorial](https://www.freecodecamp.org/news/how-to-build-a-fullstack-authentication-system-with-react-express-mongodb-heroku-and-netlify/) 
  
### *Docker*
- Install Docker for desktop
- Start Docker desktop
- In CMD check `docker --version`
- In CMD check `docker-compose --version`
- Sign up, sign in **https://hub.docker.com/**
- You want to download the PHP image for example: On the hub click on search and type PHP
- Click on the official link. go to tags and choose a recent version. for example 8.1-rc-apache
- In the CMD type: `docker pull php:8.1-rc-apache `
- To check your available images on Docker in cmd: `docker images`
- To run the image type: `run -it --name php_cont php:8.1-rc-apache /bin/bash` (You have to do this in CMD, Git-bash f.e. wont work)
- Enter, you will be on the linux machine with PHP and apache.
- `exit` to Exit
- Check running machines with: `docker ps -a`
- To stop it: `docker stop php_cont`
- To remove it: `docker rm php_cont`
- Check your PHP version in the docker: `docker run php:8.1-rc-apache php -v`
- do the same but also delete the docker process after: `docker run --rm php:8.1-rc-apache php -v`

### *PHP envirement with docker*
- Create a new folder for your project: `mkdir PHP-Example` > `cd PHP-Example`
- Create an index.php file with some `hello world`-display inside.
- Create a Dockerfile (`touch Dockerfile`). No need for extension.
- Both files in the root directory
- We are using our example image that wez pulled earlier *php:8.1-rc-apache* to create the dockerfile. 
- Create your Dockerfile. [For PHP](https://hub.docker.com/_/php)
- Dockerfile should look like : 
  ```
  FROM php:8.1-rc-apache
  COPY . /usr/src/myapp
  WORKDIR /usr/src/myapp
  CMD [ "php", "./index.php" ]
  ```
- Now you need to build the image: `docker build -t myimage .`  (Don't forget the '.')
- Run the container now with: `docker run -p 8080:80 myimage`

- *In the end just go to docker-env and do :  `docker-compose up -d ` 






