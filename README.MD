# For OPS

## Prepare
 [docs](https://moblab.atlassian.net/wiki/spaces/WEB30/pages/1682342092/Blog+Tool+-+hexo)
 
- Env
``` env
Node 12+
Git
```

- Initialize

```console
$ npm install -g hexo
$ npm install
```
- Change theme related config

  override the config in _config.yml in root folder
  `theme: cactus `

- Start server
  ```
  $ npx hexo generate // generate static files, will be at /public folder
  $ npx hexo server   // host the blog locally at http://localhost:4000
  ```

## Publish Project
- Config Git Pages
  [Git pages Guide](https://docs.github.com/en/pages/quickstart)
  config in _config.yml
  ```
  deploy:  // config for "hexo deploy", this will upload the static files to the configed repo
    type: git
    repo: https://github.com/parmeus/blog
    branch: main
    message: <any>
  ```
- Deploy
  ```
  $ hexo deploy  #need git username/password or config git ssl
  ```
  
## For Creating New Blogs
#### Use Local Env to Publish
- prepare env as for OPS
   
- write blog
  ```
  # this will create a new markdown in /source/<layout>  default is _post
  $ hexo new [layout] <title>
  $ hexo generate 
  ```
- publish to Git pages
   [refer to For OPS Publish](#publish-project)


#### Just use Markdown
  write a blog with Markdown and send it to engineering team help to publish.
  
  if you need to pre-check your markdown layout, you can use [this site](https://markdownlivepreview.com/)
  