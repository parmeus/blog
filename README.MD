# For OPS

### Prepare
 [docs](https://moblab.atlassian.net/wiki/spaces/WEB30/pages/1682342092/Blog+Tool+-+hexo)
- Env
``` env
Node 12+
Git
```

- Initialize
```console
$ npm install -g hexo
$ npx hexo init <folder>
$ cd <folder>
$ npm install
$ git clone https://github.com/probberechts/hexo-theme-cactus.git themes/cactus
```
- Set the cactus theme
  override the config in _config.yml in root folder
  `theme: cactus `

- Start server
  ```
  $ npx hexo generate
  $ npx hexo server
  ```

### Publish Project
- Config Git Pages
  [Git pages Guide](https://docs.github.com/en/pages/quickstart)
  config in _config.yml
  ```
  deploy:
    type: git
    repo: https://github.com/<username>/<username>.github.io
    branch: main
    message: <any>
  ```
- Deploy
  ```
  $ npm install hexo-deployer-git --save
  $ npx hexo deploy  #need git username/password or config git ssl
  ```
  
# For Content
#### Use Local Env to Publish
- prepare env as for OPS
   
- write blog
  ```
  # this will create a new markdown in /source/<layout>  default is _post
  $ npx hexo new [layout] <title>
  $ npx hexo generate 
  ```
- publish to Git pages
   [refer to For OPS Publish](#publish-project)


#### Just use Markdown
  write a blog with Markdown and send it to engineering team help to publish
  