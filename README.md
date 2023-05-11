# Netlore - Simple and lightweight web engine and browser.

## Navigation
- [Abstract](#abstract)
- [Goals](#goals)
- [Components](#components)
- [What will I use to create it?](#what-will-i-use-to-create-it)
- [To Do list..](#to-do-list)
- [Documentation](#documentation)

## Abstract

Netlore is a simple lightweight browser and web engine written in C. Netlore is a passion project, intended to be a fun teaching tool with which I can learn about the internals of web browsers. Writing a web browser with complete support for modern web standards is nearly impossible for an individual, so that is not the goal for this project, at least with the current number of contributors. 

## Goals

- HTML 4.0 Compatibility
- Simple CSS 2.0 (or 3.0) support
- Support a JavaScript engine (i.e NodeJS or V8)
- Good looking UI
- Handwritten HTML, CSS Parser
- Have fun!

---

## Components

Netlore will by divided into various component, each of which is responsible for a part of Netlore's functionality. All components will be hosted in [this repo.](github.com/netlore-org/netlore) Here is the list of components:

- **Netlore** (Browser)
    - **Bolly** (Web engine)
        - **Heimdall** (UI & Window Manager) - a simple UI & Window Manager library. Handles all render calls.
        - **Njord** (HTML, CSS Parser) - lexical scanning and parsing of HTML and CSS. returns a DOM element
        - **Balder** (URL Parser) - URL parser that returns a simple structure with URL
        - **Loki** (Rendering Engine) - Loki would look at DOM tree and say:
            
            > “That’s pretty easy, let’s show it on the screen.. I will just call Heimdall”
            > 
        - **Freja** (Network caller) - Handles networking and requests.
    - **Fredric** (Build system.. Why would it have even a name lol?)

---

## What will I use to create it?

| Component type | Name | Programming Language | Libraries |
| --- | --- | --- | --- |
| UI & Window Manager | Heimdall | C | SDL2 SDL_image |
| HTML, CSS Parser | Njord | C | None |
| URL Parser | Balder | C | None |
| Rendering Engine | Loki | C | None |
| Network caller | Freja | C | CURL |
| Sound | Aegir | C | libsndfile, OpenAL |
| Build system | Fredric | Makefile, Python | None (is there even a library for Makefile lmao) |

  *As you see i really like C :3*

---

## To do list..

- [ ]  **Heimdall** (UI & Window Manager)
    - [X]  *Create simple Window creator*
    - [X]  *Simple rendering system*
    - [ ]  *UI Manager*
    - [ ]  *UI Components*
        - [ ]  *Inputs*
        - [ ]  *Buttons*
        - [ ]  *Menu*
        - [ ]  *Text*
- [ ]  **Njord** (HTML, CSS Parser)
    - [ ]  *HTML Parser*
    - [ ]  *CSS Parser*
    - [ ]  *Create DOM nodes from them*
- [ ]  **Balder** (URL Parser)
    - [ ]  *Is URL correct*
    - [ ]  *Parse URL into structure*
- [ ]  **Loki** (Rendering Engine)
    - [ ]  *Render DOM*
- [ ]  **Freja** (Network caller)
    - [ ]  *Request HTTPS host and get the HTML*
    - [ ]  *Websocket*
- [ ]  **Aegir** (Sound player)
    - [ ]  Setup libsndfile
    - [ ]  Play sound by using OpenAI
- [ ]  **Fredric** (Build system)
    - [ ]  *Toolchain installer*
        - [ ]  *SDL2*
        - [ ]  *CURL*
    - [ ]  *Build whole engine*

---

# Documentation

### Notion.so version [here!](https://wild-curler-b6f.notion.site/Netlore-Simple-lightweight-experimental-browers-0640eac76821466fa6ea76a22e59dd1d)
