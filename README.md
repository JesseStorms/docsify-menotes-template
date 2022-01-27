# Docsify Menotes Template

A [Docsify.js](https://docsify.js.org) template for taking notes and summaries, based on my own setup.

## Quickstart

>I assume you've already installed [Docsify here](https://docsify.js.org/#/quickstart?id=quick-start)!

On Github: click on **Use this template:**

Afterwards; clone your own repo and run `docsify serve`

Open http://localhost:3000 (port 3000 by default) and start editing this document! Docsify automatically reloads as you save

Afterwards: change some variables found in `index.html`!

```js
 window.$docsify = {
      name: 'A new name',
      repo: 'you/your-repo-name',
      loadSidebar: true,
      themeColor: '#E00049',
      subMaxLevel: 4,
      tabs: {
        persist    : true,      // default
        sync       : false,      // default
        theme      : 'material', // default
        tabComments: true,      // default
        tabHeadings: true       // default
      }
    }
```

After that; you're set. Check out the [Example Notebook](example/) for some ideas and read up on [docsify's documentation](https://docsify.js.org)!

## Extra stuff

You can do some cool stuff when working with markdown and Docsify, thanks to pretty great community support.  
You can see some examples by checking out the [Example Notebook](example/), since I've written this page without any plugins/docsify features.

### Plugins

>You can find a complete list of plugins and themes [here](https://docsify.js.org/#/awesome)!

You can expand Docsify by using plugins! Here are some of my favorites

- [docsify-example-panels](https://github.com/VagnerDomingues/docsify-example-panels)
  - Represent content in a side-by-side fashon.
  - *Included in this repository!*
- [docsify-tabs](https://github.com/jhildenbiddle/docsify-tabs)
  - Stick content in tabs; saving space in the process.
  - *Included in this repository*
  - *Note: it messes with markmap a bit*
- [docsify-copy-code](https://github.com/jperasmus/docsify-copy-code)
  - Copy your own codeblocks easily.
  - *Included in this repository!*
- [docsify-corner](https://github.com/Koooooo-7/docsify-corner)
  - Customize the top-right corner.
- [docsify-darklight-theme](https://github.com/boopathikumar018/docsify-darklight-theme)
  - Darkmode for late-night writing.

### Generating mindmaps

Thanks to [markmap.js](https://markmap.js.org/), you can automatically generate mindmaps from your Markdown documents. There's even a Visual Studio Code extention available [here](https://marketplace.visualstudio.com/items?itemName=gera2ld.markmap-vscode). This could be useful to visualize your notes during studies.

There are some caviats with Markmap! It doesn't parse some elements, like text. It also expects your documents to be written without too many issues; like having comments directly ontop of titles.

This file is should be fully compatible with markmap!

### Deploying on Docker

You can build and deploy this repository using Docker by running

```sh
$ docker build -t notes:latest . #build the image
$ docker run --rm --name notes -d -p 80:80 notes:latest #container is running on host:80. It'll remove itself if it stops running
```

#### GitLab CI

There's an included GitLab CI file in the repository which builds, pushes to a GitLab registry and deploys it on a server using `curl`. This might be useful if you're able to host your notes somewhere using Docker.

## Contributing

Always welcome! Fork and make a pull request with your changes or make a issue and I'll get back to you.

### Contact

If there's something wrong, or you have some questions, let me know! You can find my email on my GitHub profile.