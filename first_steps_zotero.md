<!--

title: "First steps with Zotero"  

author: Damien Belvèze

date: january 2025

email: damien.belveze@univ-rennes.fr 

attribute: [First steps with Zotero](https://liascript.github.io/course/?https://raw.githubusercontent.com/damienbelveze/CFCB_IA/main/deroule_cours.md#1) 
        by [Damien Belvèze](damien.belveze@univ-rennes.fr) 
        is licensed under [CC-by-sa](https://creativecommons.org/licenses/by-sa/4.0/?ref=chooser-v1)

language: fr 

link: lia.css

icon: ./images/etoile.png

comment: this guide is adapted to PhD students who discover the free reference manager Zotero. Much of its content comes from the Zotero workshop libguide published by Formadoct and archived on [Internet Archive](https://web.archive.org/web/20210622005132/https://formadoct.doctorat-bretagneloire.fr/zotero_workshop/introduction)

import: https://raw.githubusercontent.com/LiaTemplates/citations/main/README.md

@onload
// this shall load an entire file at starttime that can be referenced
setTimeout(() => { window.bibliographyLoad("https://raw.githubusercontent.com/LiaTemplates/citations/main/bibtex.bib")}, 100)
@end

-->

# What is a reference manager

![](images/working.png)

<!--image made with the help of an AI tool for the website Formadoct on Callisto, Viêt Jeannaud -->

before reference managers exist, writers had to manualy manage their references in their manuscript. It was a very tedious and painful task (and error-prone!)

bibliographic management styling was something that used to be treated just before the milestones were reached. How many difficult nights were spent and lost in putting all references in the right place and in the right format. 

All of this now is 99% supported by this class of software named reference managers. There are several of them. Among the most popular : 

- [Refworks](https://en.wikipedia.org/wiki/RefWorks) (owned by Clarivates through Proquest)  
- [Endnote](https://en.wikipedia.org/wiki/EndNote)(also Clarivate's property and neither free-to-use nor premium)  
- [Mendeley](https://en.wikipedia.org/wiki/Mendeley) (owned by Elsevier, free-to-use) 
- and of course Zotero which is free-to-use but above all *free* [¹]

---
[¹]: [free as in freedom not as "free coffee"](https://sagitter.fedorapeople.org/faif-2.0.pdf)

# Why you should install Zotero rather than another reference manager?

If you are member of a school or laboratory which has subscribed to a proprietary software (such as Refworks or Endnote), maybe you have access to one of them. Good for you! But how will you manage your references when you are no longer member of this team?

Don't worry, it is possible to export all your references from Refworks or Endnote and to import them into Zotero. 

From Mendely you just have to export you whole library in a bib or RIS format and to import it in Zotero as it is.

For Endnote and Refworks, we could not test it on our own, but we rely for that on our colleagues from USA : 

- [importing from Refworks](https://libguides.uta.edu/zotero/importing-refworks-data-into-zotero)  

- [importing from Endnote](https://ask.lib.vt.edu/faq/38201)


# How to install Zotero

Installation process is different according to your Operating System (OS)

## Windows 

go to the download page of the [zotero website](https://zotero.org)
Download 1. the software 2. the plugin for your browser

## MacOs 

go to the download page of the [zotero website](https://zotero.org)
Zotero client embeds the plugin for Safari (you do not need to load a plugin for Safari). If you prefer to use another browser than Safari (let's say Chrome or Firefox), download and install the appropriate plugin.

## Chromebook

First you need to activate the Chromebook Linux sub-system (WSL) and then follow the instructions for GNU/Linux operating system 

## GNU/Linux 

go to the download page of the [zotero website](https://zotero.org)
download the archive (something like Zotero-6.0.35_linux-x86_64.tar.bz2)
move this file to opt/
you will need sudo rights for that. 
go to opt/
*untar* this file : 

```shell
$ tar -xf Zotero-6.0.9_linux-x86_64.tar.bz2
```

rename the resulting file : 

```shell
$ mv Zotero-6.0.9_linux-x86_64 Zotero_linux
```
*cd* within Zotero_linux

```shell
$ cd Zotero_linux
```

at this stage it's already possible to run Zotero (from this place Zotero_linux, with the following command : ./zotero), but obviously it's easier to use a desktop icon. 

Run the launcher icon under Zotero_linux : 

```shell
$ ./set_launcher_icon
```
shortcuts are usually located in ~/.local/share/applications/

So we will have to make a symlink (symbolic link) from this place to the place where Zotero Is 

```shell
$ ln -s /opt/Zotero_linux/zotero.desktop ~/.local/share/applications/zotero.desktop
```
from now you should be able to start Zotero from an icon in your application menu. 

don't forget to install the Zotero plugin in your favorite browser afterwards

## and on my smartphone

A Zotero exists in [iOS](https://www.zotero.org/support/ios). 
You may sync your Zotero library with a [beta app](https://play.google.com/store/apps/details?id=org.zotero.android&hl=en-US) designed for Android users as well. 
References may be added manually, via a DOI/ISBN or by scanning a barcode (EAN for books), but in december 2024, it was still impossible to make the Android mobile version work with a browser ([due to a lack of interoperability of Android, according to Zotero developers](https://forums.zotero.org/discussion/comment/480563#Comment_480563))


# Why should I create an account to use Zotero

you don't have to to use Zotero localy, but we strongly advise you to create an account.
This will make possible to store your data and PDFs remotely so that: 

- if you use anoter computer, you will be able to retrieve from your library online all the references you need povided you have an internet connection  
- if your computer crash or if you wipe by mistake all the data you have in your Zotero library, this data can still be found and downloaded from your online library
- Online libraries make it possible to work with other users on shared bibliographies

how to create an account? Nothing more easier, go to https://www.zotero.org/ click on login and then register, follow the instructions.
If you have already installed Zotero on your computer, just click on the Sync tab and then login with your new credentials.

![](images/sync.png)

# How does Zotero look like on my laptop

<iframe width="900" height="349" src="https://damienbelveze.github.io/first_steps_zotero/zotero_dashboard.html" frameBorder="0" scrolling="no" styles="width:100%"></iframe>











