# ThirdFlow Plugin Development Support Plugin

![Third Flow emblem](third-flow.png)

The Third Flow plugin brings to you another way to develop customizations for TiddlyWiki 5. It is not enforcing
a specific development flow, it simply tries to help you. Otherwise, it tries to stay out of your way.

* You can **develop your plugin directly from within your browser**. A server-based
TiddlyWiki instance running on Node.js ensures that all your source tiddlers are neatly stored in a clean and
hierarchically organized folder structure.

* **Source code management is done as usual** using your favorite source code management tool, such as git and others.
As the Third Flow plugin structures your tiddler source files you get a well-organized repository structure at
no price.

* For **packaging your plugin** you finally simply run a shell script which packs the plugin tiddler and saves it
to disk. Additionally, a demonstration TiddlyWiki is also created that guides your future plugin users through
the process of deploying your new plugin.

Of course, the Third Flow has been developed using the same process it supports. We actually eat our own dog food.

## In Simple Pictures

From the «a single figure lies more than a thousands words» department...

### Development Phase

![Development Phase](https://raw.githubusercontent.com/TheDiveO/ThirdFlow/master/art/ThirdFlow%20Architecture%20Development%20Phase.jpg)

### Release Phase

![Release Phase](https://raw.githubusercontent.com/TheDiveO/ThirdFlow/master/art/ThirdFlow%20Architecture%20Release%20Phase.jpg)

## Installation

```
git clone https://github.com/TheDiveO/ThirdFlow.git
cd ThirdFlow
npm install tiddlywiki
```

Then make sure, that your PATH variable is set to find the tiddlywiki binary at: `./node_modules/.bin`
or
You can install TW globally with:  `npm install -g tiddlywiki`

For Windows users the PATH variable is well hidden, so just [ask the search engine :)](https://www.google.at/search?q=How+to+set+the+path+and+environment+variables+in+Windows)

## Creating Your New Plugin

Simply copy the contents inside the `skeleton` folder to a new folder. Then start the develop phase as described next and edit and rename the plugin tiddlers as suitable for your new plugin creation. After that, simply enter the release phase. These two phases are described next. And if you need to see a full blown life demonstration then simply look at the *Third Flow* plugin itself. Enjoy!

## Starting the Server

```
develop [[username] [password]] [IP]
```

and open [localhost:8080](http://localhost:8080)

## Creating the Release Files

```
release
```

The files will be crated in then `editons/release` folder

## License

The Third Flow plugin is covered by the following licenses:

* The **Third Flow plugin** is licensed under the [MIT license](http://opensource.org/licenses/MIT).

* The **hierarchical file system adapter** is licensed under the
[TiddlyWiki 5 license](https://raw.githubusercontent.com/Jermolene/TiddlyWiki5/master/licenses/copyright.md)
(links to GitHub TW5 repository). It bases on filesystemadaptor.js and brings in storing tiddlers into hierarchical
folder structures according to their titles.

* **Other content** of this TiddlyWiki which is not part of the plugin or TiddlyWiki 5 is covered by the
[CC BY 3.0](http://creativecommons.org/licenses/by/3.0/) license.

## Author

[TheDiveO on GitHub](https://github.com/TheDiveO)
