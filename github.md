1. github的源代码管理
2. github的页面管理

#### github的实质
1. 客户计算机与服务器之间同步文本文件；
2. 将知识库作为静态页面




#### `git`命令行
1. git remote -v
2. git remote rm destination
3. git remote -v
4. git push -u origin --all
5. git remote add origin https://username@gitlab.com/group/subgroup/project.git


#### gh-pages
1. [Creating a Website on GitHub Pages](https://www.codecademy.com/article/creating-a-website-on-github-pages), setup default repository for a {username}, [Create a new repository](https://github.com/new) with repository name `{username}.github.io`, public, where {username} is your GitHub `username`; setup  GitHub Pages section; Readme.md as a default page; 
2. [Deployment of React Application using GitHub Pages](https://www.geeksforgeeks.org/deployment-of-react-application-using-github-pages/), Prerequisites, A GitHub account, Node.js and npm installed, Basic knowledge of React and Git; `git remote add origin https://github.com/<username>/<rep Name>.git`, `npm install gh-pages --save-dev`; package.json file, `"homepage": "https://<Username>.github.io/<Repository-name>"`, `"deploy": "gh-pages -d build"`, `"predeploy": "npm run build"`, `npm run deploy`; 


#### 本地`PAT`设置
1. 在`Github`中获得`PAT`, `GitHub Settings > Developer Settings > Personal Access Tokens`
2. 在本地计算机上设置`PAT`,  `git remote set-url origin https://<YOUR_GITHUB_USERNAME>:<YOUR_PAT>@github.com/danwca/portfolio.git`
3. 检查本地设置，`git remote -v`, 结果显示：`origin  https://<YOUR_GITHUB_USERNAME>:<YOUR_PAT>@github.com/danwca/portfolio.git (fetch)` 和 `origin  https://<YOUR_GITHUB_USERNAME>:<YOUR_PAT>@github.com/danwca/portfolio.git (push)`; 


#### 域名关联设置
1. 主要逻辑， 在`Github`侧设置与`repository`关联的域名， 在域名服务器侧设置域名的`CNAME=danwca.github.io`， 这样域名被解析到`danwca.gitub.io`， `Github`根据域名索引到所访问域名相应的`repository`;   
2. 一部分设置包括在`Github`的`Repository`的设置中， 另一部分设置需要在域名服务器上完成； 

#### `Github`域名控制权的验证
1. `Github`需要对所响应的域名的控制权进行验证， 以保证对所设置的域名的所属权的验证
2. 验证方法， Github会要求在域名服务器上设置相应的属性及属性值， 只要`Github`可以获得域名相应的属性及属性值， 即认可对域名的控制权； 
3. 需要根据`Github`的`Repository`的设置信息对域名服务器进行设置
