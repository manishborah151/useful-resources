# Deploying  a react app to Github(Vite)
1.  Create a github repo.
2.    ``` /vite.config.js
        base: "/ <repo_name>",
      ```
3.    ```  /package.json
            "homepage": "https://manishborah151.github.io/<repo_name>",
              "scripts": {
              "predeploy":"npm run build",
              "deploy":"gh-pages -d dist"
          },
      ```
4.  ```npm
        npm i gh-pages
    ```


5.  ```npm
      git init 
    ```
6. ```npm
      git add . 
   ```
7.   ```git
      git commit -m "first commit"
      git branch -M main
      git remote add origin https://github.com/manishborah151/<repo_name>.git
      git push -u origin main
     ```
8. ```npm
      npm run deploy
   ```

8. if need to update url
   ```
      git remote set-url origin https://github.com/manishborah151/<repo_name>.git
   ```
   
