# Multi Repo Git

A very simple Git command line tool, to manage multiple git repositories at once.

# Why you need it?

If you manage projects using multi-repo style，or worked in a micro service environment, you have most likely been asked to worked with dozen of projects.

This tool amis to replace this:

```
cd ./project1
git pull
cd ./project2
git pull
cd ./project3
git pull

```

by that:

```
mrgx git pull
```

# Getting started

## Installing

`npm install mrgx -g` will install a `mrgx` command on your system.

## Configuration

mrgx will try to read its configuration file from the current command execution path to the ancestor root path.


The configuration file must be named `.mrgx.config.json` and be in `json` format. Its best to user it in the root directory,such as `/Users/liufang/.mrgx.config.json`

```
{
    "projects":[
        {
            "path":"/Users/liufang/Neteasework/front-study"
        },{
            "path":"/Users/liufang/Neteasework/front-study-web"
        },{
            "path":"/Users/liufang/Neteasework/front-study-course"
        },{
            "path":"/Users/liufang/Neteasework/front-study-order"
        },{
            "path":"/Users/liufang/Neteasework/front-yooc"
        },{
            "path":"/Users/liufang/Neteasework/edu-front-2.0"
        },{
            "path":"/Users/liufang/Neteasework/front-study-wap"
        }
    ]
}
```

## Working with mrgx

When you're done configuring, you can use it directly on any path, just like git command itself.

![img](http://edu-image.nosdn.127.net/b22c8e19f0164cdea002b65c69b678d9.png?imageView&quality=100)

or

![img](http://edu-image.nosdn.127.net/b364fdc02c1647288d53460d31aecbab.png?imageView&quality=100)



# Want to contribute?

At this stage, the tool configuration is very simple and the function is very simple. Any idea to improve this project would be greatly appreciated.