---
title: "My favorite VSCode Extensions"
subtitle: "A list with my favorite VSCode Extensions." 
header:
  teaser: /assets/images/gallery/mohammad-rahmani-oXlXu2qukGE-unsplash.jpg
tags:
  - vscode
  - ide
  - extensions
  - productivity-developer
---
<a href="https://https://code.visualstudio.com/">VSCode</a> is one of the most popular IDE nowadays. I tried to list here the best and productivity extensions based in my own experience. Also I'll try to keep this list up-to-date.

{% capture fig_img %}
![VisualStudioImage]({{ "/assets/images/gallery/mohammad-rahmani-oXlXu2qukGE-unsplash.jpg" | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>Photo by <a href="https://unsplash.com/@afgprogrammer" target="_blank">Mohammad Rahmani</a> on <a href="https://unsplash.com/" target="_blank">Unsplash</a>.</figcaption>
</figure>


### 1. VIM (vscodevim)
<a href="https://marketplace.visualstudio.com/items?itemName=vscodevim.vim" target="_blank">VSCodeVim</a> is a Vim emulation for Visual Studio Code. That's not have all Vim features but is good enough.


### 2. Code Spell Checker

<a href="https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker" target="_blank">Code Spell Checker</a> is VSCode extension to help catch common spelling errors. In my case I also have <a href="https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker-portuguese-brazilian" target="_blank">Brazilian Portuguese - Code Spell Checker</a>.

![Image](https://raw.githubusercontent.com/streetsidesoftware/vscode-spell-checker/main/images/example.gif "Code Sepll Checker Example")

### 3. Github Copilot

<a href="https://marketplace.visualstudio.com/items?itemName=GitHub.copilot" target="_blank">GitHub Copilot</a> is an AI pair programmer which suggests line completions and entire function bodies as you type. Unfortunately access to this extension is limited a small group. If you don't have access to the technical preview, you will see an error when you try to use it. 

### 4. Thunder Client

I'm a big fan of Postman, but with <a href="https://marketplace.visualstudio.com/items?itemName=rangav.vscode-thunder-client" target="_blank">Thunder Client</a> I have the main Postman features without change my IDE.

![Image](https://github.com/rangav/thunder-client-support/blob/master/images/thunder-client.gif?raw=true "Thundler Client Example")

### 5. Docker for Visual Studio Code

The <a href="https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker" target="_blank">Docker extension</a> makes it easier to build apps that leverage Docker containers. The extension helps scaffold needed files, build Docker images, debug your app inside a container, and an explorer that makes it easy to take actions on containers and images such as start, stop, inspect, remove, and more. 

Despite not using all feature because I prefer to use command line, this extension is very useful to add in your vscode.

![Image](https://github.com/microsoft/vscode-docker/raw/HEAD/resources/readme/overview.gif "Docker Example")


### 6. Draw.io integration

<a href="https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio" target="_blank">Draw.io</a> extension is an unofficial extension integrates <a href="https://app.diagrams.net/" target="_blank">Draw.io</a> (also known as diagrams.net) into VS Code.

![Image](https://github.com/hediet/vscode-drawio/raw/HEAD/docs/demo.gif "Draw.io Example")

### Conclusion

I wrote this article in order to preset useful vscode extensions. I believe this is a work-in-progress, so I'll keep improve this post soon.