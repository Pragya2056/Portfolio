## NPM: World’s Largest Software Registry  
![npm install](https://miro.medium.com/max/1050/1*lYUy9md-knU4bRbbjjjV7A.jpeg)


We might have heard about the npm install many times. But how many of us are familiar with the topic? In this article, we will have a basic introduction to the npm install. 
npm stands for Node Package Manager maintained by npm, Inc. which is nothing but a software package manager for the JavaScript runtime environment – Node JS. Sir Isaac Z. Schluetar and his friends developed the npm registry and released it in January 2010. It is free to use and can download any public packages without registration or login. 

### What can you do with npm?

1.	You can install a new package from the registry. 
2.	You can discover or publish your own node packages. 
The online database of public and paid packages has a command-line client called npm. Some companies use them for private development and the open-source developers use them to share the software they made or the ones already in existence. There are more than 800,000 code packages in the npm registry. You can access them according to your needs and they can be easily browsed and searched on the npm website. 
There are three components in the npm package manager. They are: - 
1.	The Website
This allows you to find the third-party packages, set up profiles, and manage your package. 
2.	npm CLI 
This is a Command Line Interface that runs from a terminal allowing you to interact with npm. 
3.	Registry
This is the large public database of Javascript code. 
npm gets installed when you install Node.js on your device. And to install the CLI, you must go to your terminal and type the following code: - 

#### `npm`

Now, to check the version of your npm, type

#### `npm -v`

It isn’t a compulsion to login in the registry, but you can still do it if you want. But first, you need to check if you are already logged in. To do that, use the following command: - 

#### `npm whoami`

If you are not logged in and you want to, use the following command: - 

#### `npm login`
#### `username: <username>`
#### `password: <password>`

### package.json?

package.json is a very important topic to familiarize yourself with when learning npm. This is a plain text file with some information that npm uses to identify the project and handle dependencies. Every project in npm has a package.json file lying in its root directory. 
To create the package.json file, you need to go to the root directory of the project and execute the following command: - 

#### `npm init`

This command initializes the package.json file and prompts you for the project information using the following parameters: -
1.	Package Name
2.	Version 
3.	Test Command
4.	Git Repository
5.	Keywords
6.	Author
7.	License
As you hit enter, you will notice that the default values are accepted and then you can move on to the next prompt. Before you enter the value, you can see the default options which you can use with the help of the following command.

#### `npm init --yes`

Later, you can change the default values in package.json. 

### How to install something?

To install a new package, use the following command,

#### `npm install <package name>`

Example: - 
1.	If you want to install express, you need the following command: - 

#### `npm install express`

2.	If you want to install joi, you need the following command: - 

#### `npm install joi`

If you want a specific version of the package, you can add it in the command or if you don’t mention the version, it will download the latest one. 
To save some typing, you can use the short version of npm install: - 

#### `npm i <package name>`

You can also install multiple packages with a solo command line,

#### `npm install express joi mongo`

This will install three packages – Express, Joi, and Mongo together via a single command. 
Likewise, to install a directory, you can use, 

#### `npm install <folder name>`

When the installation is completed, there will be a new directory called /node_modules which will lie under the root of the project. In this directory, you will find all the new modules that you install. The dependencies of the above-installed packages and the dependencies of those dependencies will also be here. 

#### NOTE: - 
If you don’t know the name of the package, you can search for them on the npm website. 
Next, if you visit the package.json file, you can see that the dependencies section is updated. 

#### `"dependencies":{`
#### `"express":^4.17.1"`
#### `}`

You can also download the packages as a development dependency. This means that the package will run only in the development environment. Where your application will not work without the dependencies packages, the devDependencies will be only there during your developing period. For this, you need to use the following command: - 

#### `npm install <package name> --save -dev`

For example, if you want to install the Morgan package that logs HTTP requests, then 

#### `npm install morgan --save -dev`

The above command not only installs the morgan package but adds a new devDependencies section to the package.json file. You can view it in the file as: - 

````"devDependencies":{
    "morgan":"^1.10.0"
    }````

The packages we use as the devDependencies are not installed when we use an optional production flag. For example, linters is a package we use for enforcing clean code but is not required in production. 
While we are on the topic, the npm install with production uses the following command:

#### `npm install --production`

In short, you can write, 

#### `npm install -p`

This command when executed, there will be no installation of dependencies listed under the devDependencies section. 
There is an npm install command with –save, 

#### `npm install express -save`

This manipulates the package.json file with the intention of including the specified package as a dependency. Like on the example of the express above, the package will be added as a dependency to package.json. It can come in handy if you want future installs to include that specific package. 
Now, you can use the npm install command to download and install all packages on the dependencies and devDependencies section. 

#### `npm install`

Moving on, if you want to install a package that can be reused across the projects or if they provide executable commands from the CLI, then install them globally. However, you can install them locally if they are to be used on a single application that you are working on. When you install a package globally, the package gets installed in two places: - 
1.	In the root directory where package.json is defined.
2.	On the global node_modules folder on the user system. 
To install a package globally, use the following command: - 

#### `npm install <package name> --global`

Or, you can use the short form, 

#### `npm i <package name> -g`

npm install can run with or without the arguments. 

### Without arguments

If the npm install runs without arguments, it downloads the dependencies defined in the package.json and then generates a node_module folder with installed modules. These installed modules are placed on the node_module folder that must have the same location as package.json. Then, package.json determines what modules will get installed in the node_module folder. 
Further, you will notice a package-lock.json file that describes the dependency tree that we installed. This file is generated because it would be followed by the subsequent installs to use the exact same tree. This is regardless of the intermediate dependency updates. 

### With arguments 

When you run npm install with arguments, it downloads everything from the before specified location to the original node_modules directory at the project root. There will be no new node_modules folder inside the sub-directory but thy will be hoisted to the node_modules folder at the root of the project directory. 
Moving on, npm install can run with git as well. For this example, let’s take Vows, a Node.js testing framework that can be installed from git alongside its single dependency – eyes. 

#### `git clone http://github.com/cloudhead/vows`
#### `cd vows`
#### `npm install`

Now, let’s see how you can share your own software in the npm registry. You can just sign in at the [npm registry](www.npmjs.com) website. 

Further, navigating to your project and publishing this project can be done like this: 

#### `c:\users\myuser>cd myproject`
#### `c:\users\myproject>npm publish`

### Security Concerns

npm relies on the NoSQL Couch DataBase to manage the publicly available data. There have been some issues with the npm install a few times. 
1.	A npm package was taken down by an author in 2016 which was then used by thousands of developers. It has such a big impact that an entire community was brought down. 
2.	Google found an abuse with a fact that the node_module can act on user systems which leads to republishing and changes in the packages from that user. This can affect thousands of developers across the world. 

### Are there any alternatives?

We have some good alternatives to npm in the market. They show compatibility with the public npm registry and use it by default. However, they provide different client-side experiences that focus on performance and determinism when compared with the npm client. 
At JSconf 2019, npm’s former CTO announced a new federated package registry, Entropic. It is mainly aimed at the decentralization of JavaScript commons and is Apache 2 licensed as well. 
Likewise, other alternatives of npm are: -
1.	ied
2.	pnpm
3.	npmd
4.	Yarn
The last one, Yarn was released by Facebook in October 2016 and is really gaining popularity among developers. 

