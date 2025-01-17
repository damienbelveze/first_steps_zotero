this guide is adapted to PhD students who discover the free reference manager Zotero. Much of its content comes from the Zotero workshop libguide published by Formadoct and archived on [Internet Archive](https://web.archive.org/web/20210622005132/https://formadoct.doctorat-bretagneloire.fr/zotero_workshop/introduction)

# How to access the resource from the repository

To display the lesson in your browser, click on the link below

[![course badge](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://raw.githubusercontent.com/damienbelveze/first_steps_zotero/main/first_steps_zotero.md#1)

Liascript is a markdown interpretor created by [André Dietrich](https://liascript.github.io/authors/andre-dietrich/)


# Licence 

This work is licenced under the Creative Commons CC:by Licence 

# How to edit this guide 

In order to edit this guide, download the files, open the file "first_steps_zotero.md".
The document is written in markdown format, a format readable in any text editor. 
In order to edit and visualize changes in the same time, we suggest you use [VScode editor](https://code.visualstudio.com/). 
The two Liascript plugins designed for VSCode (Liascript-Preview and Liascript-Snippets), are not yet available for Codium, VSCode's open source alternative.

- install VSCode
- install Liascript-Preview and Liascript-Snippets plugins
- open the folder that contains first_steps_zotero.md file (trust the authors)
- define this folder as your workspace 
- in VScode, open the palette (Ctrl+shif+P)
- in the palette search for "Open User Settings (JSON)" File, open this json file. 
- in this file, add the following snippet: 

```json

"[markdown]": {
        "editor.tabCompletion": "on",
        "editor.quickSuggestions": {
            "comments": "on",
            "strings": "on",
            "other": "on"
        },
        "editor.snippetSuggestions": "top"
     }

```
- close this file, go back to first_steps_zotero.md 
- make the changes you need
- to see the changes online, whenever you want, open your browser, type http://localhost:8000/ in your adresse bar 
- from VScode, type Alt+L, in the localhost tab, you shoud see a menu displayed with a list of files 
- select first_steps_zotero.md, the preview of your course should be displayed 

Liascript documentation is [available in english from Liascript github repository](https://github.com/liaScript/docs), an interactive version (live editor with documentation) is available [here](https://liascript.github.io/LiveEditor/?/edit/GSaCieV1bPVXUYEuoOU0TCZa). Click on the rocket icon to open the whole documentation. 

# How to get an URL for this course from your repository 

This repository can be stored on a server you use or in a forge (github, gitlab)
If you use github as a forge, copy the link to your markdown document (for instance http://github.com/username/liascript_project/course.md)
go to the [Liascript website](https://liascript.github.io/) and put the URL in the "enter-your-markdown-url-here" field. 
You should get the URL to share with your attendants. 

