# Programming-Journal
This repo is a log of what I'm programming daily. 

## 4/29/2023
-Created the store page and shopping cart of a website using React.js, React-router, and typeScript.  
-Need to add local storage connection 
## 4/30/2023
-Added local storage to the store page. 
-finished this project since only wanted to practice store page setup with Typescript & React for future e-commerce applications.
-created a repo called "React-Typescript-Shopping-Cart"

## 5/07/2023
 I decided to read the dev.java docs, download the JDK, and write my first Java program. I learned the syntax, how to compile etc, knowing OOP in javascript made the process a lot easier. 

## 5/23/23
 -Working on the Mattermost open-source app, the issue request for a component to be transferred from jsx to tsx, and make all the necessary adjustments and testing (if applicable) that goes with that.  So far I've changed the file extension to tsx and adjusted the extension in the files the component was imported into.  The component was utilizing PropType for React, I was thinking since that is used to double-check data type that I would need to remove it since typescript is being used.  However, since proptype checks the type at runtime and typescript at compilation I wasn't sure if I should keep it in.  I googled it and the StackOverflow suggested a babel plugin "babel-plugin-typescript-to-proptypes" that generates proptypes from typescript interfaces and type aliases.  To double-check I asked in the contributor forum and someone suggested the plugin as well so I went ahead and checked to see if the plug-in was already installed in the app, and it was.  I added an interface to the component and removed the static prototype. 
 
 ## 5/24/23
 -Added another interface for value and text  and one for error.  The value and text interface was added to the props interface.  I did this in order to use it in the handleChange function for the newValue data type. Then in the variable already in the function that stores a map of the newValue I added (newValue as Option[]).map...  I copied the change and pasted it on ChatGPT, and asked it to explain the code to me - I did this to check if my train of thought was correct, and it was. 
 -Got an error on the onChange ```No overload matches this call``` imported the ValueType from react-select and assigned it as the parameter's data type which fixed the problem. 
 
 ## 5/30/23
 -On Friday I sent another comment to the review of my draft PR regarding the package-lock.json.  When I first sent the draft PR with questions, he commented that I needed to revert the package-lock.json.  I didn't even know I made any changes on there but it seems that when I npm installed the clone on my local computer the dependencies were updated.  The updates were too many for me to manually go one by one to update the file, so I looked online to see if there was a way to do this.  I was about to ask the contributor but decided to call my friend who is a senior swe and he was perplexed as well but mentioned there are symbols you can add to a dependent version to prevent its update.  That was not going to work for me since that meant I would still have to go one by one to do that, but it did make me think that if that is the case then maybe npm install might have something, so I went to the npm install docs and found that there is "--no-package-lock" option that can be added to the npm install command that will keep the existing lock file as is.  I ended up not using that, I had commented back to the draft PR reviewer asking what his suggestion was and he said to do it manually by copying and pasting the package-lock.json file from the master branch. Man...why the heck did I not freaking think of that- Now I know. 
 
 
 -Submitted my pull request with the changes, waiting for review. 
 
 # 6/2/23
-I didn't add a release note to the OG PR request because since there were not any I assumed I didn't need to include it, but it turns out that I needed to include it anyway as "release note/none"  Also I title needed to match the issue, the reviewer changed the title for me.  I commented back my apologies for not doing those two things and I got this comment back. "Please know that there is absolutely no need to apologize. The work and time contributors like you have dedicated to this are truly invaluable, and I want to express my utmost appreciation for your efforts."  This made my day, no my whole week.  I suggested little optimizations plus I fixed some linter spacing errors and the PR should be good to go.  I pushed a commit to the PR for review. Once this is done I'll be starting on a C++ open source contribution. 

# 7/03/23

-(written on 9/24) Working on a client's website, it's a local Dominican restaurant that wants an interactive website where users can see the menu, make reservations, and see current Yelp reviews.  We discussed the details, we agreed on a WordPress website in order for him to add new updates to the page himself once I complete the website and teach him how to do so.  sent him a contract to sign and it was and we are good to go. 

# 8/20/23
 - (backlog, written on 9/25) Have most of the website done, added a video of the restaurant to it and it looks great.  WordPress is a lot more fun than I thought it would be, I still prefer to fully code websites for clients but the plugins and themes in WordPress have been fun, and I learned a lot.  I did code some CSS for a few custom buttons so there was code in there.

# 9/4/23
-(backlog, written on 9/25) The website has been completed but still waiting for the client to give final approval since he's been out of the country for some time. 

 # 9/24/2023
 -I started a new project using next.js for the frontend and Node/Express for the back end.  I read through the docs and followed the tutorial in Next.js docs and it was very well done with a lot of details. However, I still thought it was a replacement for Express, so I was having a hard time figuring out how to create my project.  The personal project I'm working on is a health insurance proposal generator with 3 fictitious insurance plans available that users can select from.  The target market is health insurance brokers who would like to create a quote for their clients who are businesses looking for insurance for their employees. Therefore, I need to create a backend that will generate the API that will be used to create the proposal for companies.  I couldn't figure out how to do that just using Next.js, I had already set up the database with Supabase and was researching why it just didn't seem like I was reading Next.js docs correctly.  Then on YouTube, I found "Next.js Tutorial for Beginners| Next.js 13 by programming with Mosh and that's when I finally understood that Next.js is only for frontend! I still have to create the Node/Express backend server for this project.  I'm so excited to have a clear plan now for how to structure the project. 

  # 10/12/2023
  -Created a table in Supabase(PostgreSQL) for the health insurance plans, and added all the necessary columns except for the premiums.  since it will be age-banded I have to create a separate premium per age group, was trying to alter the table to add these columns, but was having a little issue with it.  Looked through the Postgresql docs and I think the issue is that the data type I was using (decimal(10,2) doesn't exist in Postgresql, will look more into it. 

 # 10/15/2023
  -I have entered all three medical insurance plans into postgreSQL in Supabase.  It was not an easy task since the table had 22 columns.  I decided to create all the rows using the SQL editor except for the Bronze plan.  For that one, I used the table editor instead.  
