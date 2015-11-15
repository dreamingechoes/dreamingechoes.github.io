---
layout: post
title:  "Consuming a RESTful API faster with AngularJS and Yeoman."
date:   2015-11-15 15:30:00
categories: angularjs yeoman api
tags: angularjs yeoman api development web
comments: true
excerpt: "Find the perfect shop near you when you are in a hurry and need something is important, so today we're gonna do a geosearch example to help our users and make their lives easier..."
post_summary: "Find the perfect shop near you when you are in a hurry and need something is important, so today we're gonna do a geosearch example to help our users and make their lives easier..."
image:
  feature: header-image.png
  main: /images/2015-11-15-consuming-a-restful-api-faster-with-angularjs-and-yeoman/title.png
url: /angularjs/yeoman/api/consuming-a-restful-api-faster-with-angularjs-and-yeoman/
---

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## First step: install all the dependencies

Let's just get into it. First thing you we'll need is have `node.js` installed on your system. If you don't have it, go to [https://nodejs.org](https://nodejs.org) and install it. After that, we have to install Yeoman, and in order to do that, execute the following instruction on your terminal (maybe you'll need to execute it as a root user):

```sh
user@computer:~$ npm install -g yo
```

The `-g` flag tells `node.js` to install Yeoman globally on your system. It's very important to use this flag because if we don't specify, it's going to be installed locally in the folder you are and you won't be able to run it as a command. Then, let's install [generator-webapp](https://www.npmjs.com/package/generator-webapp), which is a Yeoman generator that scaffolds out a frontend web app:

```sh
user@computer:~$ npm install -g generator-angular
```

Due to we're going to use `sass`, we have to install `compass` too. Follow the steps of the official web [here](http://compass-style.org/install/). Finally, let's install `grunt` and `bower`:

```sh
user@computer:~$ npm install -g grunt
user@computer:~$ npm install -g bower
```

## Making our AngularJS app with the Giphy API

With that done, we're able to create a folder for our application and execute inside it the `yo` command to generate our scaffold application:

```sh
user@computer:~$ mkdir angularjs_giphy_app
user@computer:~$ cd angularjs_giphy_app
user@computer:/angularjs_giphy_app$ yo angular
```

`yo` is going to ask you some questions in order to create our application. We only have to respond the rest of the questions. Here are my elections:

```sh
? Would you like to use Gulp (experimental) instead of Grunt? No
? Would you like to use Sass (with Compass)? Yes
? Would you like to include Bootstrap? Yes
? Would you like to use the Sass version of Bootstrap? Yes
? Which modules would you like to include? angular-animate.js, angular-cookies.js, angular-resource.js...
```

After the process has finished, just execute `grunt serve`, and what that's going to go it's going to start up a web server on your own computer using `node.js` and it's going to open a web browser with your application. You'll see something like this:

![screenshot](/images/2015-11-15-consuming-a-restful-api-faster-with-angularjs-and-yeoman/screenshot1.png)

Bla bla bla...

## Any place where I can see the result?

Yeah! Here you have the [Github repo](https://github.com/dreamingechoes/geosearch_with_mongodb) for this example, so you can clone it, change it, play with it... whatever you want! :)
