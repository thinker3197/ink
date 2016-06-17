---
title: Sublime Build System
---

<p class="lead"> <a href="http://jekyllrb.com">Jekyll</a> is a static site generator, an open-source tool for creating simple yet powerful websites of all shapes and sizes.</p>

[Sublime Text](https://www.sublimetext.com/) is one of the most popular editors out there and it's loved by developers. We'll talk about sublime and it's build system today. A brief note of what build system is and how to create your own build system for any language.

## What are build systems?

> Build system builds and run programs using external programs. 

Using sublime build systems we can build/run any program without leaving the editor. For understading, think of what you'll do to build a JavaScript file. You'll hop into the terminal and type in ```node yourFileName.js``` and node will build the js file for you. Sublime build system exactly do the same thing, but without having you to leave the editor. Sublime comes pre-loaded with few build systems for Python, Ruby, C++ etc. You can view them in **Tools > Build Systems** menu in sublime.

## Creating a build system

If you try to build a program whose build system does not exist, the sublime won't be able to build it. This is beacuse sublime dosen't know which program to choose to build this particular file. Hence by **Creating a build system**, we aim to tell sublime to use a particular program to build a certain type of file. To create a build system for any language in sublime go to **Tools > Build System > New Build System**. In sublime build system files are stored with extension ```.sublime-build```. For an example I'll create build system for for a few languages. All we need to create a build system is write the shell command that is needed to build that file and the selector that will let sublime know to use this build system on what kind of files.

#### JavaScript

```javascript
{
	"shell_cmd": "node $file",
	"selector": "source.js"
}
```
#### CoffeScript
```javascript
{
	"shell_cmd": "coffee -c $file",
	"selector": "source.js"
}
```
#### Grunt
```javascript
{
    "shell_cmd": "grunt --no-color",
    "selector": ["source.js", "source.less", "source.json"]
}
```
#### Jade
```javascript
{
    "shell_cmd": "cmd /c jade $file",
    "selector": "source.jade"
}
```
#### Stylus
```javascript 
{
    "shell_cmd": "stylus $file",
    "selector": "source.stylus"
}
```   

Creating build systems for commonly used programming languages increases productivity and automation and hence is worth a shot. For any queries related to this post, hit me a [mail](mailto:ashishgupta.3197@gmail.com)
