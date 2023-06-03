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
 
 ## 5/24/23
 -Added another interface for value and text  and one for error.  The value and text interface was added to the props interface.  I did this in order to use it in the handleChange function for the newValue data type. Then in the variable already in the function that stores a map of the newValue I added (newValue as Option[]).map...  I copied the change and pasted it on ChatGPT, asked it to explain the code to me - I did this to check if my train of thought was correct, and it was. 
 -Got an error on the onChange ```No overload matches this call``` imported the ValueType from react-select and assigned it as the parameter's data type which fixed the problem. 
 
 ## 5/30/23
 -On Friday I sent another comment to the review of my draft PR regarding the package-lock.json.  When I first sent the draft PR with questions, he commented that I need to revert the package-lock.json.  I didn't even know I made any changes on there but it seems that when I npm installed the clone on my local computer the dependencies where updated.  The updates were too many for me to manually go one by one to update the file, so I looked online to see if there was a way to do this.  I was about to ask the contributer but decided to call my friend who is a senior swe and he was perplexed as well but mention there are symbols to you can add to a dependecy version to prevent it's update.  That was not going to work for me since that means I will still have to go one by one to do that, but it did make me think that if that is the case then maybe npm install might have something, I so I went to the npm install docs and found that there is "--no-package-lock" option that can be added to the npm install command that will keep the existing lock file as is.  I ended up not using that, I had commented back to the draft PR reviewer asking what his suggestion was and he said to do it manually by coping and pasting the package-lock.json file from the master branch. Man...why the heck did I not freaking think of that- Now I know. 
 
 
 -Submitted my pull request with the changes, waiting for review. 
 
 # 6/2/23
-I didn't add a release note to the OG pr request because since there were not any I assumed I didn't need to include it, but it turns out that I needed to include it anways as "release note/none"  also I title needed to match the issue, the reviewer changed the title for me.  I commented back my apologies for not doing those two things and I got this comment back. "Please know that there is absolutely no need to apologize. The work and time contributors like you have dedicated to this are truly invaluable, and I want to express my utmost appreciation for your efforts."  This made my day, no my whole week.  I suggestings little optimimizations plus I fixed some linter spacing errors and the pr should be go to go.  I push a commit to the pr for review. Once this is don't I'll be starting on a c++ open source contribution. 
 
 
