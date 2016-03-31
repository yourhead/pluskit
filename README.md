# PlusKit
### A multi-tool for your RapidWeaver site
#### originally by LogHound
Create mashups with your RapidWeaver pages and give them extra abilities.

![PlusKit Icon](https://raw.githubusercontent.com/yourhead/pluskit/master/assets/icon_256.png)


## Download
 - [Stable Release v2.92.1](https://github.com/yourhead/pluskit/raw/master/downloads/PlusKit_2.92.1.zip)
 - [Beta Release v3.0.0 beta 2](https://github.com/yourhead/pluskit/raw/master/downloads/PlusKit_3.0.0b2_1095.zip) - [Release Notes](http://yourhead.com/appcast/RW6/PlusKit/release_notes_3.0.0b2_1095)


### From the LogHound site

PlusKit is a new type of RapidWeaver® plugin. Traditionally plugins have added new pages styles (such as Sitemap or Blocks), PlusKit is a different. PlusKit gives every page in your RapidWeaver site more power.

 - It can automatically convert your photos to 'lighbox' or 'FancyZoom' format (this is super-slick)
 - It provides a powerful importing function (@import(())), from any Styled Text you can import another RW page
 - A great use for this is if you want your Rapidflickr photos inside a sidebar, or perhaps you want an Accordian in a sidebar
 - It provides a useful global find feature. Good for tracking down where things went
 - Seamlessly integrate Google Docs & Spreadsheets
 - It makes your Style better with powerful new tags (<bash>, and <markdown>)
 - Plus much more -- You might want to watch the screencast here to get a better sense.
 - Feel free to download a trial version of pluskit. The 'free' version works for 10 minutes before disabling itself, to allow it to work more than 10 minutes you can purchase a license at the Loghound.com store.





## StylePlus

StylePlus adds several new tags within StyleText and allows you to 'import' other pages from within RapidWeaver.

The tags are:

 - markdown
 - bash
The arguments you can pass are (default in bold)

 - cache=default \| none \| always
 - warning=true \| false
 - timeout = 5 \| (some number of seconds)
 - files=_FILES_ | (something else that you want to refer to remove files with)
 - outputdir= (some local directory you want copied to the server)

If you are just getting started you can ignore the arguments (or said another way you will know when you need them)

### Markdown
A simple markdown example

```
<markdown>
*Hello from Markdown*
</markdown>
```

Yields

*Hello from Markdown*
You can read more about markdown Syntax by going to John Gruber's "Main Site" here

### Bash
The next one to focus on is the 'Bash'. This is pretty cool since you know now execute arbitrary code when viewing a page. There are lots of uses for this but for now let's do something trivial

```
<bash>
echo -n "the current date is:"
date
</bash>
```

Yields

echo -n "The current date is:" date

### Import
Finally let's talk briefly about the 'import' feature. This is pretty slick and allows you to include pages within pages

For instance:

```
@import((Home))
```

would include the contents of your 'Home' page inline -- A very powerful way to combine multiple page types.










## Find


PlusKit also includes a new powerful find feature. Ever wonder where something was in your RapidWeaver project? Wonder no more!



You can locate FindPlus in the 'Edit -> Find Plus'













## Google Docs


PlusKit allows you to integrate documents from Google Docs. This allows for a sort of 'mini CMS' system where you can have portions of your web site that can be edited by anyone, anywhere in the world and the changes show up instantly on your web page. 

To integrate a document look at the gdoc command. 

To integrate a spreadsheet look at the gtable command -- as opposed to gdoc, gtable is a fairly complex command and usually takes a bit more work (due to the extra complexity of how to display tables)

There is also the gform command for doing forms and storing the results in your google spreadsheet (great for surveys)

This feature requires PHP support (so no .mac)
