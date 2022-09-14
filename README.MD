
# The Parmeus Blog

Updates, ideas and inspiration from Parmeus

  

## Local installation

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

$ hexo generate // generate static files, will be at /public folder

$ hexo server // host the blog locally at http://localhost:4000

```
Each time you have a change on local file and want to check the result, you should run ```hexo generate``` and refresh your ```http://localhost:4000``` page
  

## Write new post

this will create a new markdown file in /source/<layout> default layout is _post

```$ hexo new [layout] <title>```

```$ hexo generate```
  

#### Just use Markdown

write a blog with Markdown and send it to engineering team help to publish.

if you need to pre-check your markdown layout, you can use [this site](https://markdownlivepreview.com/)