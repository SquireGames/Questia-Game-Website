---
author: Matthew Kaminski
title: What Questia is, its History and its Future
---

Questia is a 2D action-adventure game primarily centered around questing and boss fighting.
However, unlike many of the similar games currently available, Questia will feature a unique character leveling up system
  and will be online multiplayer.
As much as I would like to delve into specifics about the game, Questia is still very early into development and will not
  be complete for a while.
The game, along with its engine, just recently started being rewritten from the ground up, but earlier versions of the project
  are still available in the [Play]({{ site.baseurl }}{% link play.md %}) page. 
If you are interested in contributing to this project, anybody at any skill-level can send me a message via the contact information
  provided in the [About]({{ site.baseurl }}{% link about.md %}) page.


## Development and Design 

Some of the technical design goals for the project include:
- following modern C++ coding practices
- following the best git practices
- being completely open source
- supporting all major operating systems
- having sufficient code and design documentation
- having unit and continuous integration testing
- providing enough abstraction/modularity to be able to change dependencies with little friction
- use zero-cost abstraction for performance-critical code

Additionally, the technologies that we currently use are:
- Programming Languages
  - C++17 for the game and engine
  - CMake for build scripts
  - Python for automation and package management
- Build tools
  - CMake for building the project
  - Conan for package management
- Libraries
  - GLFW for creating windows, OpenGL contexts, and handling input
  - Glad for the GL load-generator
  - GoogleTest for testing and mocking
- Potential future dependencies
  - UltraLight for UI
  - Crypto++ for encrypting and hashing
  - Google protobuf for class serialization
  - Valve GameNetworking Sockets for network communications
  - JSON for Modern C++
  - OpenAL for audio
  - Docker for server management

The goal of the underlying engine will be to create a flexible but targeted environment to create specific types of 2D games. 
Questia Engine is _not_ meant to replace existing game engines and libraries such as SFML, Godot, Unity, or GameMaker Studio,
  but rather is meant to build an efficient and multiplayer-capable framework for specifically envisioned projects. 


## History

The origin of Questia dates all the way back to the end of 2014, when I wanted to embark on a simple project
  shortly after I had just started teaching myself programming.
Questia was inspired by the various other games I played at up to that time, namely Runescape until '07, Might 
  and Magic III, Puzzle Pirates, Mabinogi until '12, and Realm of the Mad God until '13.
Over the years, the project underwent multiple near-complete rewrites and changes.
The build environment changed from Code::Blocks to makefiles, transitioned once again to CMake, and then incorporated the Conan package manager. 
Questia used various dependencies over the years, including Boost, Cryptopp, Angelscript, SFML, SDL, and UnitTest++.
The original code and builds are still available on the _Play_ page, and the original repositories are still found in the GitHub organization.
Here are some old screenshots of Questia:

{% include post_image.html url="2019-03-23/Main_Menu.png" description="Old Main Menu" %}
{% include post_image.html url="2019-03-23/In_Game.png" description="A goblin killing a chicken" %}
{% include post_image.html url="2019-03-23/In_Game_2.png" description="Shooting an arrow at a house" %}
{% include post_image.html url="2019-03-23/Map_Editor.png" description="Old Map Editor" %}
{% include post_image.html url="2019-03-23/Old_Website.png" description="Old Website" %}
 