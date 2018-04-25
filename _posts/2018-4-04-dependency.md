---
layout: post
title: blog10
---
# Dependency
Lately i've been doing a lot of coding in javascript, specifically for node.js as opposed to for a website directly. With this comes the inevitable use of [npm](https://www.npmjs.com/). npm is Nodes package manager, and its honestly one of the best package managers I've ever used. No need to carry around all of your project dependencies with your code either in your repository or somewhere else, all you need to do is list a dependency your project has and run npm install. It even takes care of installing dependencies for your dependencies! So convenient, right?

Right, it is convenient, but it's easy to not realise exactly how many packages your using. I installed 8 packages for a project (including some of the bigger ones like react and express) and wound up with my dependency folder (called 'node_modules') full of over 60 sub folders, each one representing a node package. This is a ridiculous amount of packages installed, but I don't really need to know what they do as long as the main packages I installed work. Unfortunately, I may need to know what they do if I want to put a specific type of open source licence on my project. In that case, I would need to make sure my license is compatible with the licenes of each project that I'm making use of. This can be a nightmare, and might even turn some people away from releasing open source software.

Luckily, GitHub has decided to come to the (rescue)[https://www.cbronline.com/news/github-gives-businesses-helping-hand-open-source-project-licensing]. Github has released, completely open source, its application called (Licensed)[https://github.com/github/licensed] to help with keeping track of the licenses of dependencies. Github currently uses this code themselves, and have made it open to the world with a disclaimer that it is not a one stop shop for licensing needs. Even so, it's a huge boon to any business who wants to better keep track of their license dependencies for any of 6 popular package managers (Bower, Bundler, Cabal, Go, Manifest lists, and NPM). While this software will not solve the problem of overuse of project frameworks (sometimes equivalent to using a steam roller to roll your dough, it'll work but it's overkill), it will at least help those currently navigating this jungle of dependencies to better be able to release open source software.