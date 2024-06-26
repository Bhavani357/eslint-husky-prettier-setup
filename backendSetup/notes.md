## Backed eslint-husky-prettier Setup 
* `npm init -y`
* `npm i husky lint-staged prettier eslint --save-dev` 
* `git init`
* `npx husky init`
* `npm init @eslint/config`
  - How would you like to use ESLint?
   - To check syntax and find problems
   - JavaScript modules (import/export)
   - which framework? none 
   - does your project use typescript? yes
   - where does your code run? nodejs 
   - would you like to install them now? yes 
   - which package manager do you want? npm

* add lint-staged code in package.json file 
```json 
 "lint-staged":{
    "*.js":["prettier --write","eslint --fix", "git add ."]
 }
```

* create server.js file write code 
* create `.gitignore` file and from toptal copy paste the gitignore file code 
* open eslintrc.js file add `env:{..., commonjs:true}`