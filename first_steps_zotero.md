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

# First steps with Zotero

```ascii

          _____                   _____                   _____                   _____            _____                            _____            _____                   _____                   _____                   _____                  
         /\    \                 /\    \                 /\    \                 /\    \          /\    \                          /\    \          /\    \                 /\    \                 /\    \                 /\    \                 
        /::\    \               /::\    \               /::\    \               /::\    \        /::\    \                        /::\    \        /::\    \               /::\    \               /::\    \               /::\    \                
       /::::\    \              \:::\    \             /::::\    \             /::::\    \       \:::\    \                      /::::\    \       \:::\    \             /::::\    \             /::::\    \             /::::\    \               
      /::::::\    \              \:::\    \           /::::::\    \           /::::::\    \       \:::\    \                    /::::::\    \       \:::\    \           /::::::\    \           /::::::\    \           /::::::\    \              
     /:::/\:::\    \              \:::\    \         /:::/\:::\    \         /:::/\:::\    \       \:::\    \                  /:::/\:::\    \       \:::\    \         /:::/\:::\    \         /:::/\:::\    \         /:::/\:::\    \             
    /:::/__\:::\    \              \:::\    \       /:::/__\:::\    \       /:::/__\:::\    \       \:::\    \                /:::/__\:::\    \       \:::\    \       /:::/__\:::\    \       /:::/__\:::\    \       /:::/__\:::\    \            
   /::::\   \:::\    \             /::::\    \     /::::\   \:::\    \      \:::\   \:::\    \      /::::\    \               \:::\   \:::\    \      /::::\    \     /::::\   \:::\    \     /::::\   \:::\    \      \:::\   \:::\    \           
  /::::::\   \:::\    \   ____    /::::::\    \   /::::::\   \:::\    \      \:::\   \:::\    \    /::::::\    \               \:::\   \:::\    \    /::::::\    \   /::::::\   \:::\    \   /::::::\   \:::\    \   ___\:::\   \:::\    \          
 /:::/\:::\   \:::\    \ /\   \  /:::/\:::\    \ /:::/\:::\   \:::\____\ /\   \:::\   \:::\    \  /:::/\:::\    \          /\   \:::\   \:::\    \  /:::/\:::\    \ /:::/\:::\   \:::\    \ /:::/\:::\   \:::\____\ /\   \:::\   \:::\    \         
/:::/  \:::\   \:::\____/::\   \/:::/  \:::\____/:::/  \:::\   \:::|    /::\   \:::\   \:::\____\/:::/  \:::\____\        /::\   \:::\   \:::\____\/:::/  \:::\____/:::/__\:::\   \:::\____/:::/  \:::\   \:::|    /::\   \:::\   \:::\____\        
\::/    \:::\   \::/    \:::\  /:::/    \::/    \::/   |::::\  /:::|____\:::\   \:::\   \::/    /:::/    \::/    /        \:::\   \:::\   \::/    /:::/    \::/    \:::\   \:::\   \::/    \::/    \:::\  /:::|____\:::\   \:::\   \::/    /        
 \/____/ \:::\   \/____/ \:::\/:::/    / \/____/ \/____|:::::\/:::/    / \:::\   \:::\   \/____/:::/    / \/____/          \:::\   \:::\   \/____/:::/    / \/____/ \:::\   \:::\   \/____/ \/_____/\:::\/:::/    / \:::\   \:::\   \/____/         
          \:::\    \      \::::::/    /                |:::::::::/    /   \:::\   \:::\    \  /:::/    /                    \:::\   \:::\    \  /:::/    /           \:::\   \:::\    \              \::::::/    /   \:::\   \:::\    \             
           \:::\____\      \::::/____/                 |::|\::::/    /     \:::\   \:::\____\/:::/    /                      \:::\   \:::\____\/:::/    /             \:::\   \:::\____\              \::::/    /     \:::\   \:::\____\            
            \::/    /       \:::\    \                 |::| \::/____/       \:::\  /:::/    /\::/    /                        \:::\  /:::/    /\::/    /               \:::\   \::/    /               \::/____/       \:::\  /:::/    /            
             \/____/         \:::\    \                |::|  ~|              \:::\/:::/    /  \/____/                          \:::\/:::/    /  \/____/                 \:::\   \/____/                 ~~              \:::\/:::/    /             
                              \:::\    \               |::|   |               \::::::/    /                                     \::::::/    /                            \:::\    \                                      \::::::/    /              
                               \:::\____\              \::|   |                \::::/    /                                       \::::/    /                              \:::\____\                                      \::::/    /               
                                \::/    /               \:|   |                 \::/    /                                         \::/    /                                \::/    /                                       \::/    /                
          _____                  \_____/           _____ \|___|            _____ \/____/                    _____                  _______          _____                   ______/                 _____                  _______/                 
         /\    \                 /\    \          /\    \                 /\    \                          /\    \                /::\    \        /\    \                 /\    \                 /\    \                /::\    \                 
        /::\____\               /::\    \        /::\    \               /::\____\                        /::\    \              /::::\    \      /::\    \               /::\    \               /::\    \              /::::\    \                
       /:::/    /               \:::\    \       \:::\    \             /:::/    /                        \:::\    \            /::::::\    \     \:::\    \             /::::\    \             /::::\    \            /::::::\    \               
      /:::/   _/___              \:::\    \       \:::\    \           /:::/    /                          \:::\    \          /::::::::\    \     \:::\    \           /::::::\    \           /::::::\    \          /::::::::\    \              
     /:::/   /\    \              \:::\    \       \:::\    \         /:::/    /                            \:::\    \        /:::/~~\:::\    \     \:::\    \         /:::/\:::\    \         /:::/\:::\    \        /:::/~ \:::\    \             
    /:::/   /::\____\              \:::\    \       \:::\    \       /:::/____/                              \:::\    \      /:::/    \:::\    \     \:::\    \       /:::/  \:::\    \       /:::/  \:::\    \      /:::/    \:::\    \            
   /:::/   /:::/    /              /::::\    \      /::::\    \     /::::\    \                               \:::\    \    /:::/    / \:::\    \    /::::\    \     /::::\   \:::\    \     /::::\   \:::\    \    /:::/    / \:::\    \           
  /:::/   /:::/   _/___   ____    /::::::\    \    /::::::\    \   /::::::\    \   _____                       \:::\    \  /:::/____/   \:::\____\  /::::::\    \   /::::::\   \:::\    \   /::::::\   \:::\    \  /:::/____/   \:::\____\          
 /:::/___/:::/   /\    \ /\   \  /:::/\:::\    \  /:::/\:::\    \ /:::/\:::\    \ /\    \                       \:::\    \|:::|    |     |:::|    |/:::/\:::\    \ /:::/\:::\   \:::\    \ /:::/\:::\   \:::\____\|:::|    |     |:::|    |         
|:::|   /:::/   /::\____/::\   \/:::/  \:::\____\/:::/  \:::\____/:::/  \:::\    /::\____\        _______________\:::\____|:::|____|     |:::|    /:::/  \:::\____/:::/__\:::\   \:::\____/:::/  \:::\   \:::|    |:::|____|     |:::|    |         
|:::|__/:::/   /:::/    \:::\  /:::/    \::/    /:::/    \::/    \::/    \:::\  /:::/    /        \::::::::::::::::::/    /\:::\    \   /:::/    /:::/    \::/    \:::\   \:::\   \::/    \::/   |::::\  /:::|____|\:::\    \   /:::/    /          
 \:::\/:::/   /:::/    / \:::\/:::/    / \/____/:::/    / \/____/ \/____/ \:::\/:::/    /          \::::::::::::::::/____/  \:::\    \ /:::/    /:::/    / \/____/ \:::\   \:::\   \/____/ \/____|:::::\/:::/    /  \:::\    \ /:::/    /           
  \::::::/   /:::/    /   \::::::/    /       /:::/    /                   \::::::/    /            \:::\~~~~\~~~~~~         \:::\    /:::/    /:::/    /           \:::\   \:::\    \           |:::::::::/    /    \:::\    /:::/    /            
   \::::/___/:::/    /     \::::/____/       /:::/    /                     \::::/    /              \:::\    \               \:::\__/:::/    /:::/    /             \:::\   \:::\____\          |::|\::::/    /      \:::\__/:::/    /             
    \:::\__/:::/    /       \:::\    \       \::/    /                      /:::/    /                \:::\    \               \::::::::/    /\::/    /               \:::\   \::/    /          |::| \::/____/        \::::::::/    /              
     \::::::::/    /         \:::\    \       \/____/                      /:::/    /                  \:::\    \               \::::::/    /  \/____/                 \:::\   \/____/           |::|  ~|               \::::::/    /               
      \::::::/    /           \:::\    \                                  /:::/    /                    \:::\    \               \::::/    /                            \:::\    \               |::|   |                \::::/    /                
       \::::/    /             \:::\____\                                /:::/    /                      \:::\____\               \::/____/                              \:::\____\              \::|   |                 \::/____/                 
        \::/____/               \::/    /                                \::/    /                        \::/    /                ~~                                     \::/    /               \:|   |                  ~                       
         ~~                      \/____/                                  \/____/                          \/____/                                                         \/____/                 \|___|                                           
                                                                                                                                                                                                                                                    
```

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


For which Operating system you need information to install Zotero?

- [ ] Windows
- [ ] MacOS
- [ ] VanillaOS (Chromebook)
- [ ] GNU\Linux 
- [ ] Android / iOS
<script output="tasks">"@input"</script>

<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[0]) {
    send.liascript(`>## Windows 

go to the download page of the [zotero website](https://zotero.org)
Download 1. the software 2. the plugin for your browser`

    )
  } else send.clear()
} catch(e) { }
</script>


<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[1]) {
    send.liascript(`>## MacOs 

go to the download page of the [zotero website](https://zotero.org)
Zotero client embeds the plugin for Safari (you do not need to load a plugin for Safari). If you prefer to use another browser than Safari (let's say Chrome or Firefox), download and install the appropriate plugin.`

    )
  } else send.clear()
} catch(e) { }
</script>

<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[2]) {
    send.liascript(`>## Chromebook

First you need to activate the Chromebook Linux sub-system (WSL) and then follow the instructions for GNU/Linux operating system` 

    )
  } else send.clear()
} catch(e) { }
</script>

<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[3]) {
    send.liascript(`>## GNU/Linux 

go to the download page of the [zotero website](https://zotero.org)
download the archive (something like Zotero-6.0.35_linux-x86_64.tar.bz2)
move this file to opt/
you will need sudo rights for that. 
go to opt/
*untar* this file : 


>>$ tar -xf Zotero-6.0.9_linux-x86_64.tar.bz2


rename the resulting file : 

>>$ mv Zotero-6.0.9_linux-x86_64 Zotero_linux

*cd* within Zotero_linux


>>$ cd Zotero_linux


at this stage it's already possible to run Zotero (from this place Zotero_linux, with the following command : ./zotero), but obviously it's easier to use a desktop icon. 

Run the launcher icon under Zotero_linux : 

>>$ ./set_launcher_icon

shortcuts are usually located in ~/.local/share/applications/

So we will have to make a symlink (symbolic link) from this place to the place where Zotero is :


>>$ ln -s /opt/Zotero_linux/zotero.desktop ~/.local/share/applications/zotero.desktop

from now you should be able to start Zotero from an icon in your application menu. 
don't forget to install the Zotero plugin in your favorite browser afterwards`

    )
  } else send.clear()
} catch(e) { }
</script>

<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[4]) {
    send.liascript(`>## and on my smartphone?

A Zotero exists in [iOS](https://www.zotero.org/support/ios). 
You may sync your Zotero library with a [beta app](https://play.google.com/store/apps/details?id=org.zotero.android&hl=en-US) designed for Android users as well. 
References may be added manually, via a DOI/ISBN or by scanning a barcode (EAN for books), but in december 2024, it was still impossible to make the Android mobile version work with a browser ([due to a lack of interoperability of Android, according to Zotero developers](https://forums.zotero.org/discussion/comment/480563#Comment_480563))`

    )
  } else send.clear()
} catch(e) { }
</script>

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


# collecting bibliographic references

Since iths 6th version, Zotero encapsulates its own PDF viewer making it possible to annotate, comment a PDF or capture and extract figures out of a it.
You are going to collect a PDF document in your Zotero library


>- save [this presentation](https://digitalrepository.unm.edu/cgi/viewcontent.cgi?article=1163&context=hslic-posters-presentations) in your Zotero library   
>- check the reference (compare it with what appears on the titlepage of the document) : what should be amended or completed ?  
>- open the PDF by double clicking on it : highlight some text, write a comment. both actions will have **annotations** as outputs  


In this case, Zotero made a request to Google Scholar and found the link to the parent citation. But sometimes, it won't be possible to retrieve any citation from Scholar or elsewhere. You will need to add it manually!


>- <a href="document.pdf" download>download this document</a>
>- import it (drag and drop it) in your library
>- open it in the PDF viewer
>- create the reference manually (title, author, date)


# How to use tags

Don't wait till your library becomes too big to be easily manageable with only collections and subcollections. In order to improve the findability of your references in your library, you should consider adding tags to your references. 

The default way of getting tags in your library is to let Zotero capture tags associated to the references in the source (database, catalog, etc.). If you prefer to deal only with tags you have chosen, you may inhibit this feature by unchecking a box in the main settings panel.
(go to edit > settings > General ; uncheck "automatically tag items with keywords and subject headiings)
If you let many of these inherited tags populate your collections, you can get rid of them in just one move : 
in the tag panel (bottom-left by clicking on the filter icon and checking the "delete automatic tags in this library" option) : 


![](images/remove_inherited_tags.png)

this can be achieved for a specific collection

If you want to tag your references, it can easily be down from the right sidebar:

!?[](gif/add_tags.mp4)

for each reference, you may add as many tags as you want. 
You may assign a specific color to 9 of your tags : this feature is pretty usefull if you need to conduct a literature review from references stored in several collections. 

> add two tags to one of your references and assign a color to each of them

# Let's talk about word processors

Zotero would not be very helpfull if it was not designed to help you insert and manage references within your word processor throughout the process of writing. 
Now, most of word processors are interoperable with Zotero but not all. 
Which one do you usually use? 

- [ ] Word from Microsoft Office
- [ ] LibreOffice
- [ ] OpenOffice
- [ ] Google doc 
- [ ] Pages from Mac
- [ ] Don't bother me with word processors, I use text editors
<script output="tasks">"@input"</script>


<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[0]) {
    send.liascript(`>## Word
    Zotero usually works well with the desktop wersion of Word (for instance Word 2021), but not with Office365. 
    As soon as you have installed Zotero, the Zotero plugin for Word might be added to this word processor. 
    It adds a tab named "Zotero" in the Word menu`
    )
  } else send.clear()
} catch(e) { }
</script>


<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[1]) {
    send.liascript(`>## LibreOffice
    Zotero usually works well with LibreOffice. In some cases, the plugin for LibreOffice won't be automatically installed on Windows because Zotero needs to connect to a Java environment and can find any on the computer.
    To install such an environment, close LibreOffice and Zotero, go to [Oracle website](https://jdk.java.net/) and download the last stable release available. Then reinstall the plugin for LibreOffice from Zotero ( Edit > Settings > Cite)
    Reopen LibreOffice, check that LO is now connected to a Java Environment (JRE, JDK or an equivalent for GNU/Linux OS) : 
     ![](images/java.png). 
    If Java is properly connected to LO, Zotero icons should be visible and active:
    ![](images/zotero_icons.png)
    `
    )
  } else send.clear()
} catch(e) { }
</script>

<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[2]) {
    send.liascript(`>## OpenOffice
    LibreOffice was born of Oracle's takeover of the OpenOffice software (and name). 
    OpenOffice is no longer updated, and is used by Oracle to create confusion with the free software suite born of OpenOffice and renamed LibreOffice in response to resistance from its original developers.
    OpenOffice may not work properly with Zotero, you'd better give up OpenOffice and switch to LibreOffice ([downloadable from here](https://www.libreoffice.org/download/download-libreoffice/))
    `
    )
  } else send.clear()
} catch(e) { }
</script>

<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[3]) {
    send.liascript(`>## Google Doc
    Experienced researchers will tell you that's not a very good idea to write a scientific text on Google Doc. Who knows what Google will make out of text and data you give access them to by using their spreadsheets and word processor?
    But if you are engaged in a collaborative writing project, Google Doc can be usefull though. Zotero references can be inserted in a Google Doc by using Google's Zotero Google Doc Integration app. 
    ![](images/google_doc_zotero.png)
    `
    )
  } else send.clear()
} catch(e) { }
</script>

<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[4]) {
    send.liascript(`>## Pages
    Pages has never been interoperable with Zotero and [is unlikely to work with this reference manager in the future](https://forums.zotero.org/discussion/102457/requesting-for-plugin-for-pages) due to choices made by the Software editor. You may connect Pages to Endnote (if you have an access to EN) but not to Zotero.
    These guys don't like Free Software. You 'd better quit Pages and opt for more transparent and interoperable products such as LibreOffice.
    `
    )
  } else send.clear()
} catch(e) { }
</script>

<script style="width: 100%">
try {
  let task = @input(`tasks`)

  if(task[5]) {
    send.liascript(`>## Don't tell me about word processors, I use a text editor
    Not only we agree, but we value this : using free text editors makes science more reproductible. Besides word processors are distraction prone compared to text editors. See below our section about text editors
    `
    )
  } else send.clear()
} catch(e) { }
</script>

> If you use a word processor that works with Zotero, check that Zotero icons are present and active (something happens iy you click on one of them)

![](images/zotero_icons2.png)

## How to insert a reference

The next activity will be divided in two parts : 

1. save references in Zotero
2. Insert them in a text 

You will be prompted to choose a bibliographic style ; choose the first one listed in the popup.

<a href="insert_references.odt> download">download this text file</a>

> - Create a new collection "word_processor"
> - Find the references listed in the document (1-6) online
> - save them in the *word_processor" collection
> - insert them in the right place in the document
> - print the bibliography at the end of the document

## How to insert a note 

Since Version 6, Zotero allows you to insert notes taken with Zotero editor as well as references

In the word processor editor, select the reference "First Experiences with Reading Primary Literature by Undergraduate Life Science Students"

> using the icons at the top of the PDF viewer, try to reproduce the get this result:

![](images/PDF_notes.png)

> convert all these "annotations" (left panel) in a single "note" 

to achieve this : right panel > notes > add note from annotations

![](images/add_note.png)

> edit this note in order to add the following paragraph:

```text
"Open archives repositories have been in existence in France since 2001; from 2006, a proactive policy led the main research agencies and universities to coordinate their actions towards a common archiving platform, HAL (Hyper Articles on Line), operated by CNRS (Centre National pour la Recherche Scientifique)"

```
> In this new paragraph, within the note add [the source of this paragraph]((https://onlinelibrary.wiley.com/doi/abs/10.1087/095315107X239636) )

(Collect this reference and add it to the note)

We will now insert our note into our document *insert_refernces.odt". Use the "insert note" button to achieve this. The note should be inserted at the end of the document, before the bibliography

> add this note and refresh the bibliography 


