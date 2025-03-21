1. github的源代码管理
2. github的页面管理

#### github的实质
1. 客户计算机与服务器之间同步文本文件；
2. 将知识库作为静态页面


#### gh-pages
1. [Creating a Website on GitHub Pages](https://www.codecademy.com/article/creating-a-website-on-github-pages), setup default repository for a {username}, [Create a new repository](https://github.com/new) with repository name `{username}.github.io`, public, where {username} is your GitHub `username`; setup  GitHub Pages section; Readme.md as a default page; 
2. [Deployment of React Application using GitHub Pages](https://www.geeksforgeeks.org/deployment-of-react-application-using-github-pages/), Prerequisites, A GitHub account, Node.js and npm installed, Basic knowledge of React and Git; `git remote add origin https://github.com/<username>/<rep Name>.git`, `npm install gh-pages --save-dev`; package.json file, `"homepage": "https://<Username>.github.io/<Repository-name>"`, `"deploy": "gh-pages -d build"`, `"predeploy": "npm run build"`, `npm run deploy`; 

