# Plan of learning
Thanks to the list in [awesome-awesomeness](https://github.com/bayandin/awesome-awesomeness). My summaries for analyzed repositories goes to my [blog](http://hustlion.github.io/).


# Codecombat
This may be better. 

Hmmm, node 0.10.x required but,,, don't want to install,,, try with 0.12

hmm, the folowing just downloaded the repo....

wget https://raw.githubusercontent.com/codecombat/codecombat/master/scripts/devSetup/bootstrap.sh
chmod +x bootstrap.sh
./bootstrap.sh git@github.com:HustLion/codecombat.git

sudo python ./coco/scripts/devSetup/setup.py

This script will set mongodb and node v0.10.x for you. Better combine this script with my script.


    ./coco/bin/coco-mongodb - Starts MongoDB
    sudo ./coco/bin/coco-brunch - Starts brunch, which watches for file changes
    ./coco/bin/coco-dev-server - Starts your local web server

http://localhost:3000/

wget http://analytics.codecombat.com:8080/dump.tar.gz
tar -xzvf dump.tar.gz
mongorestore --drop dump

Code Syncing

Pick up upstream changes:

    git fetch upstream

## First-time setup

	cd
	wget https://raw.githubusercontent.com/codecombat/codecombat/master/scripts/devSetup/bootstrap.sh
	# if necessary, modify node version to 0.12
	chmod +x bootstrap.sh
	./bootstrap.sh git@github.com:HustLion/codecombat.git
	sudo python ./coco/scripts/devSetup/setup.py
	./coco/bin/coco-mongodb 
	wget http://analytics.codecombat.com:8080/dump.tar.gz
	tar -xzvf dump.tar.gz
	mongorestore --drop dump
	sudo ./coco/bin/coco-brunch
	./coco/bin/coco-dev-server

Shoud keep `./coco/bin/coco-brunch` running in a terminal. It will automatically reload the page. Once the server successfully started with `2015-07-01T14:49:26.556Z - info: Successfully connected to MongoDB queue!`, visit `http://localhost:3000/`.

Maybe I can optimize the wiki according to this.
	

## Workflow
cd
./coco/bin/coco-mongodb
sudo ./coco/bin/coco-brunch
./coco/bin/coco-dev-server

if you want to update the database, close the server and:
	wget http://analytics.codecombat.com:8080/dump.tar.gz
	tar -xzvf dump.tar.gz
	mongorestore --drop dump
	sudo ./coco/bin/coco-brunch
	./coco/bin/coco-dev-server

## Coffee-snake - coffee script
[Coffee-snake](https://github.com/HustLion/coffee-snake) is a great successor for the [snake](## learning - Snake - Web), which has github pages and gitmodules and coffee script. Consider it as a upgrade :).

Command about **submodule** (learnt [here](http://blog.csdn.net/wangjia55/article/details/24400501)):
	git submodule update --init --recursive

* [tutorial](http://thecodeplayer.com/walkthrough/html5-game-tutorial-make-a-snake-game-using-html5-canvas-jquery)
* [The code player](http://thecodeplayer.com/): a wonderful learning site.
* [Coffee script](http://coffee-script.org/#language)
* [Atom](https://github.com/nornagon/atom): a small <canvas> framework.

## javascript_snake - web
This is with Phaser Engine. [Javascript_snake](https://github.com/HustLion/javascript_snake).

This one is quite advanced among all the 'snakes' here.

* [Phaser](http://phaser.io): A fast, free and fun open source framework for Canvas and WebGL powered browser games.
* [cocos2d-x](https://github.com/cocos2d/cocos2d-x): cocos2d-x is a multi-platform framework for building 2d games, interactive books, demos and other graphical applications. It is based on cocos2d-iphone, but instead of using Objective-C, it uses C++. It works on iOS, Android, Windows Phone and Store Apps, OS X, Windows and Linux.
* [cocos2d-html5](https://github.com/cocos2d/cocos2d-html5): Cocos2d-html5 is a cross-platform 2D game engine written in Javascript, based on Cocos2d-X and licensed under MIT. It incorporates the same high level api as “Cocos2d JS-binding engine” and compatible with Cocos2d-X. It currently supports canvas and WebGL renderer.
* [Bower](http://bower.io/): A package manager for the web.

## Coil
[Coil](https://github.com/HustLion/Coil) great UI! Sci-Fi! Great!

* a great user [Lee Reilly](https://github.com/leereilly) with a wonderful modern [site](http://hakim.se/)

## compiled - Craft - C
A sandbox game: [Craft](https://github.com/HustLion/Craft)

Easy to compile and run.

* a .gitignore file here. Good demo.


## Lila - web

A complex browser based chess game: [Lila](https://github.com/HustLion/lila)

This is really a huge one.

* [Build tutorial](https://github.com/ornicar/lila/wiki/Lichess-Development-Onboarding)
* [Node.js](https://nodejs.org/): for npm. And [Tutorial](https://github.com/workshopper/learnyounode)
* [zsh](http://www.zsh.org/): [Oh my zsh](https://github.com/robbyrussell/oh-my-zsh) and some introductory [material](http://zhuanlan.zhihu.com/mactalk/19556676)
* [sbt](http://www.scala-sbt.org/)
* [Scala 2.11](http://www.scala-lang.org/)
* [Play 2.3](http://www.playframework.com/)
* [Akka 2 actors](http://akka.io)
* [Stockfish](http://stockfishchess.org/): a chess engine.
* [MongoDB 2.6](http://mongodb.org): [Install and run](http://docs.mongodb.org/master/tutorial/install-mongodb-on-ubuntu/?_ga=1.98665310.1727689462.1435314057)
* [OpenSSL](https://www.openssl.org/)
* [nginx 1.6](http://nginx.org): [beginner guide](http://nginx.org/en/docs/beginners_guide.html)
* [mithril.js](http://lhorie.github.io/mithril/)
* [prismic.io](http://prismic.io): Free Simple repository plan for Open Source and Open Content projects. Content under this plan will be licensed under the Creative Commons Attribution 4.0 International License.

## compiled - ArxLibertatis - C++
[ArxLibertatis](https://github.com/HustLion/ArxLibertatis) is a first-person role-playing game. And there is detailed comlipling [guide](http://wiki.arx-libertatis.org/Downloading_and_Compiling_under_Linux) available, which is very helpful for me as a starter.

There are many dependencies to install which could be fun and expand my toolkit.

After compiling, I think, this is good for learning, but the quality of characters is not as high as commercial ones such as Resident Evil. It's sufficient for learning purpose, but can I find some really elegant games to learn?



### Notes:
CMakeList.txt seems quite important for cmake. Check it out later, [post](http://stackoverflow.com/questions/2601798/adding-compiled-libraries-and-include-files-to-a-cmake-project).

[Find Freetype](http://www.cmake.org/cmake/help/v3.0/module/FindFreetype.html)

The build failed with the info:

	CMake Error at /usr/share/cmake-2.8/Modules/FindPackageHandleStandardArgs.cmake:108 (message):
	Could NOT find Freetype (missing: FREETYPE_INCLUDE_DIRS) (found version 11.0.5")

To resolve it, simply use:
	sudo apt-get install 

Shortcut to toggle windowed and fullscreen mode (default is Alt+Enter) 

### Resources:
* [FreeType](http://www.freetype.org/): FreeType is a freely available software library to render fonts. Use `freetype-config` to check the version of the library that is installed on your system.
* [SDL](http://www.libsdl.org/)
* [OpenGL](http://www.opengl.org/)
* [GLEW](http://glew.sourceforge.net/)
* [OpenAL](http://kcat.strangesoft.net/openal.html)
* [zlib](http://zlib.net/)
* [Boost](http://www.boost.org/)
* [GLM](http://glm.g-truc.net/): OpenGL Mathematics
* [Qt 4.7+ or 5: QtCore, QtGui, QtWidgets (for Qt 5 only) and QtNetwork libraries](http://qt.nokia.com/)
* [GDB](http://www.gnu.org/software/gdb/)
* Run arx in a debugger, [instructions](http://wiki.arx-libertatis.org/Debugging)

### Bug found:

When the game is switched to fullscreen, the mouse moves too fast.


### Further Reading:
* [FreeType](http://www.freetype.org/) `autogen.sh`, `freetype-config` files.
* arx `arx-install-data` script, can be launched with a window, wonderful, have a look.
* arx developer doc. `make doc`->not working, `make style`-> valid. Also the [website](http://wiki.arx-libertatis.org/Developer_Information)


## Alge's Escapade
[Alge's Escapade](https://github.com/HustLion/game-off-2012), HTML5, JavaScript, GameJs arcade game where you control an Algae. 

Interesting.



## next
[Newtoon's Revenge](https://github.com/HustLion/NewtonsRevenge)
A very good manual demo [playframework manual](https://github.com/playframework/playframework/tree/2.4.x/documentation/manual)

[Avabranch](https://github.com/Zolmeister/avabranch) a snake variant.
[Heal 'em All ]() modern zombie.
Hyperspace Garbage Collector
HexGL : Sci-Fi, racing
0hh1
2048 
Monkey Rally 
Bash game: [bash2048](https://github.com/HustLion/bash2048)

# a very good example of writing articles about algorithms, [link](https://github.com/HustLion/bezierinfo)
