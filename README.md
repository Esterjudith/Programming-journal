# Programming-log
This repo is a log of what I'm programming daily. 

## 4/29/2023
-Created the store page and shopping cart of a website using React.js, React-router, and typeScript.  
-Need to add local storage connection 
## 4/30/2023
-Added local storage to store page. 
-finished this project since only wanted to practice store page setup with Typescript & React for future e-commerce application.
-created repo called "React-Typescript-Shopping-Cart"

## 5/07/2023
 -Decided to read the dev.java docs,download the jdk and write my first java program. I learn the syntax, how to compile etc, knowing OOP in javascript made the process a lot easier. 

## 5/23/23
 -Working on the Mattermost open-source app, the issue request for a component to be transfered from jsx to tsx, and make all the necessary adjustments and testing (if applicable) that goes with that.  So far I've changed the file extension to tsx and adjusted the extension in of the files the component was imported into.  The component was utilising PropType for React, I was thinking since that is use to double check data type that I would need to remove it since typescript is being used.  However, since proptype checks the type at runtime and typescript at compilation I wasn't sure if I should keep it in.  I googled it and the stackoverflow suggested a babel plugin "babel-plugin-typescript-to-proptypes" that generates proptypes from typescript interfaces and type alias.  To double check I asked in the contributor forum and someone suggested the plugin as well so I went ahead and checked to see if the plug in was already installed in the app and it was.  I added and interface to the componant and removed the static proptype. 
