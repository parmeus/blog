
  

## Non-tech user
#### Use Markdown
Write a blog with Markdown and send it to engineering team help to publish.
If you need to pre-check your markdown layout, you can use [this site](https://markdownlivepreview.com/)
You can also find this instruction with photos at [confluence page](https://moblab.atlassian.net/wiki/spaces/WEB30/pages/1691680778/How+to+use+Github+webpage+to+update+Blog)

#### New post
1. Go to directory ``source/_posts``
2. Click ``Add file`` dropdown button
3. Select ``Create new file``
4. Name the file
5. Paste below content to the top of the new file
	```
	---
	title: title of the file
	date: 2022-09-02 10:56:46 (change this to your blogging time)
	tags: tags if applies
	---
	```
6. Paste your blog markdown content right below [5]
7. Scroll down the page and edit the commit message 
8. Click ``Commit new file`` button
9. After this, automation script will handle the rest. Typically  it will take about 2-3 minutes for the new content to show up.

 #### Edit existing post
 1. Go to ``source/_posts``
 2. Click on the file you want to edit
 3. You can find a pencil like button on the top-right corner of the file, click it.
 4. Edit the content 
 5. Scroll down and edit the commit message
 6. Click ``Commit changes``


## Engineering user local installation
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

### Write new post
this will create a new markdown file in /source/<layout> default layout is _post
```$ hexo new [layout] <title>```
```$ hexo generate```
