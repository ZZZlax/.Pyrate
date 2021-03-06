# .Pyrate
A small, self-destructing Qt5 web browser written in python and designed for/with unique functions for Ubuntu.

### What do you mean self-destructing? ###
When a Qt5 web browser is launched it creates a .local file that hosts all of the cookie-cache's targeted by evercookies (aka serverside cookies). I created a function titled ".abandonShip" that removes the Qt5 folder entirely, with all of it's contents, on command. I tested it against multiple serverside cookies and have yet to find one not removed by this process. That isnt to say it isnt possible, just that, for most practical purposes this proves effective.

### What is with the .weirdLettering() ###
That is Qt5 syntax: the naming of options had more to do with saving space then trying to be "l33t".

### Ok, so what other "unique" functions are there? It's just a browser. ###
True, there isnt anything new under the sun here (besides maybe the self-destruction thing.) It is .onion enabled so if you have already downloaded Tor you can now access .onion sites in .Pyrate aswell. It has the ability to play/load/view contents through drag and drop from your home folder making it useable beyond just visiting websites. It still has bookmarks, downloads, ect.. However the way it is arranged is fairly unique:

1. I did away with the over-packed menus of other browsers and consolidated the basic functionality into 3 comboboxes and a single url bar spread across 2 toolbars. This allows you to customize the layout, to an extent, without cluttering your view with dozens of buttons and menus.
2. I never enabled redirects; I want full control of my boat in the digital ocean. You can still navigate to the redirect manually using the url bar but freedom and user control are central to the .Pyrate code.
3. I never enabled direct downloads; Pyrates pick their cargo- if not you are just a privateer. You can download anything you want with .Pyrate, you just have to copy/paste or drag/drop the link into the url bar and select '.downLoad.' under '.capsQuarters'- your options menu.
4. I made an option to generate a qr of whatever is in the url bar: url, hashes, any text from your clipboard or that you drag/dropped from a page. It is the quickest way to share information from your lap/desktop to phone without signing/setting up or logging into anyting.
5. All bookmarks are handled through saving HTML to local files. The idea was to create a form of script injection so basic and easy to access that anyone with a basic understanding of the concept and no knowledge of front end development could extract, read, copy/cut/paste and test their code all in a simple .txt format. I am fully aware that QT has an entire module for scripting- I aimed more for K.I.S.S. with the context of education in mind. If you want to add script injection features, I will leave a link to the Qt page for scripting in python and you can add it yourself or, if you would like to add to/fork this project feel free.
6. I made an option called ".djanGo()" that automates the setup of a new django web-framework project with the help of a dialogue box. Nobody ***NEEDS*** this, you should be able to handle that on your own if youre messing with django. My only reasoning is to "automate the boring stuff." Not to mention, you can self host your bookmarks, if you were so inclined.
7. This browser is not designed for the basic user: it was written on Ubuntu FOSS with FOSS at the root of the idea. It likely wont port well to other platforms without tweaking a few things but it shouldnt be a massive process to correct.
8. 'seaShanties' is a ***demonstration*** for ***educational purposes only*** of the effectiveness of paring BeautifulSoup with a search engine for quickly gathering information on a topic aswell as a basic implimentation of data transfer from one program to another using .txt (this is usually done though .csv files, but for the sake of beginner approachability I went with .txt), and the usefulness of dequing processes atexit. Also, it downloads music. (***Im not responsible if you download unauthorized songs, check your album search lists for download authorization with youtube before saving, you can always cancel the download of any video by pressing ctrl+c in your terminal if it violates copywright restrictions***)
9. Your homescreen is a local html file by default so you can copy/paste your own html onto or in place of the .Pyrate_Player.html template to customize your homescreen in a way other browsers wont let you.
10. '.hashWords' is a tool to generate hashes of web objects by copying urls, links, or strings into the url bar and hitting '.hashWords'. This is useful for quickly compairing long urls/links, or even entire bodies of text or code snippets against simular objects. (Note, hashes are salted by default in python, therefore results vary from one instance of .Pyrate to the next. Put simply: dont use '.hashWords' do generate a password no matter how much it sounds like the implied function. I assume you have seahorse or keypass.) 

### Why? ###
Occams razor: the simplest solution is the most likely one. You dont need 34mb to make a connection to a .onion website and you dont need machine learning to remove a server side cookie. If you browsing data is stored in memory, and your memory is reset when the power turns off, you automatically reset your browsing data on open/close.
No one expects you to delete firefox and use .Pyrate but if youre looking for a fun project to reverse engineer/beautify or give to your teenage relative with the clear instructions ***NOT*** to abuse downloads, this might be it.

### WTF is pip_quick? ###
Sometimes you dont want to build and install a script/package, you just want to run it quickly and put it back in storage/delete it. That is where pip_quick comes in. You can still run setup.py but if you are ok with installing the dependencies outside of the script path and managing them yourself you can clone .Pyrate and run it immediatly from whereever you cloned it- pip_quick will subprocess all of the installs for you, including the Qt5 dependencies.

### Notes: ###
*If you want access to .onion sites aswell you will need to install tor on your own. I'm not forcing it.*
*To use the '.djanGO' feature you must [duh] 'pip install django'.*


*** Work in progress, more features in beta ***
