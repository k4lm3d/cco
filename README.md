# Hello, world!
Repository by **K4LM3D**

---

## Technologies

- [**Hexo**](https://hexo.io/)
  Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

### Quick Start

#### Installation

- Install Hexo via Node.js:
```bash
$ npm install hexo
```

#### Setup (Windows 10)
  Guide: https://hexo.io/docs/setup

- Create directory for your Hexo website

```bash
$ npx hexo init <folder>

$ cd <folder>
```

- Install theme (Using Icarus)
```bash
$ npm install -S hexo-theme-icarus hexo-renderer-inferno

$ npx hexo config theme icarus
```

- Install GitHub pages deployer
  Guide: https://hexo.io/docs/github-pages

```bash
$ npm install hexo-deployer-git --save
```

## Deploy GitHub repository

``` bash
$ npx hexo clean
$ npx hexo deploy

$ npx hexo server

$ git init
$ git add *
$ git commit -m "first commit"
$ git branch -M main
$ git remote add origin https://github.com/k4lm3d/k4lm3d.github.io.git
$ git push -u origin main
```


### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

<!-- http://localhost:4000/cco/ -->

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)

___


# To create a new post or a new page, you can run the following command:

`$ hexo new [layout] <title>`

post is the default layout, but you can supply your own. You can change the default layout by editing the `default_layout` setting in `_config.yml`.

## Layout
There are three default layouts in Hexo: `post`, `page` and `draft`. Files created by each of them is saved to a different path. Newly created posts are saved to the `source/_posts` folder.

**Layout**  **Path**
`post`	    `source/_posts`
`page`	    `source`
`draft`   	`source/_drafts`

## Drafts
Previously, we mentioned a special layout in Hexo: `draft`. Posts initialized with this layout are saved to the `source/_drafts` folder. You can use the publish command to move drafts to the `source/_posts` folder. publish works in a similar way to the new command.

`$ hexo publish [layout] <title>`

Drafts are not displayed by default. You can add the `--draft` option when running Hexo or enable the `render_drafts` setting in `_config.yml` to render drafts.

## Scaffolds
When creating posts, Hexo will build files based on the corresponding file in `scaffolds` folder. For example:

`$ hexo new photo "My Gallery"`

When you run this command, Hexo will try to find `photo.md` in the `scaffolds` folder and build the post based on it. The following placeholders are available in scaffolds:

**Placeholder** 	**Description**
`layout`	        Layout
`title`	          Title
`date`	          File created date

