---
layout: post
title:  "Three.js and Cannon.js: Basic Third Person Game"
date:   2015-06-28 22:50:45
categories: Learn Browser-based Game
---

# THREE-BasicThirdPersonGame
[THREE-BasicThirdPersonGame](https://github.com/HustLion/THREE-BasicThirdPersonGame): [tutorial](http://matthiasschuetz.com/three-basicthirdpersongame/docs). Really cool. Try it [live](https://rawgit.com/HustLion/THREE-BasicThirdPersonGame/master/demo1_simple.html).

I'm interested in three.js so I will learn this one. Later learn phaser engine.

* THREE.js: [docs](http://threejs.org/docs/)
* Cannon.js: this framework is a pure math and physics collection which can do complex calculations if you want a realistic simulation. [Docs](https://github.com/schteppe/cannon.js/wiki).
* [stats.js](http://github.com/mrdoob/stats.js): JavaScript Performance Monitor. From this learnt how to write js in bookmarklet.
* [rawgit.com](http://rawgit.com/): RawGit serves raw files directly from GitHub with proper Content-Type headers. 
* [Google Closure Compiler](https://github.com/google/closure-compiler): To get the latest version of it, click [here](http://dl.google.com/closure-compiler/compiler-latest.zip). Also can get it [here](https://github.com/mrdoob/stats.js/tree/master/utils/compiler).
* [ant](http://ant.apache.org/bindownload.cgi): Apache Ant is a Java library and command-line tool that help building software.
* [emoji cheat sheet](http://www.emoji-cheat-sheet.com/)
* [highcharts](https://github.com/highslide-software/highcharts.com/)

With [rawgit.com](http://rawgit.com/), a new way to deploy my scripts to my pages: build js with closure, in html I use relative path, only in my post I use rawgit.com links. Then all the css, html, js should be automatically resolved. Actually if use my own server, I can have a cdn myself since the [source code](https://github.com/rgrove/rawgit) is available. :smiley:



# Analysis

This is constructed as a tutorial. The code of all JavaScript files is fully commented. The whole game logic is placed in the `game.core.js` file.

To start, read the [tutorial](http://matthiasschuetz.com/three-basicthirdpersongame/docs). With this it's not difficult to understand the game.

So we start with `demo1_simple.html`, `WebGL` gets checked and then the game is initiated. `Stats` monitors the frame rate and the game goes into the `loop()`. 

I read the details and found some libs there. And I think it's mostly variable definitions and functions which comply with physic laws. In this project, for now I think there is no game engine like phaser applied. So I think I will just examine the 3D part and write about it in my post and then I go to the phaser project.

In `game.three.js`, the `render()` function is defined, which turns out that it's just a callback. The `createModel()` is the one I care about. It imports json data and deal with it. Ok, the model is imported by the code beginning at line 83 of `game.core.demo1`. The json data is stored in `game.models.js`. This file is really just a model, with lots of data. After importing, the script adds material and mesh to it.

# Summary
From this repo I acquired better understanding of a common game frame: `Init`->`Setup`->`Loop`. Found some wonderful tools like [rawgit.com](http://rawgit.com/), [stats.js](http://github.com/mrdoob/stats.js), [emoji cheat sheet](http://www.emoji-cheat-sheet.com/). From the details of code, I found that physics formulae are applied heavily. Maybe it's time to check out how real game engines deal with these tasks.

# Further Reading
* Similar repo with also tutorials: [BuildNewGames_ThreeJSGame forked from nklsrh/BuildNewGames_ThreeJSGame](https://github.com/HustLion/BuildNewGames_ThreeJSGame)
