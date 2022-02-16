# School Attendence Website

Website: [https://esmelillywhite.github.io/websiteESRC/](https://esmelillywhite.github.io/websiteESRC/)

Editted from lab journal template: [https://crumplab.github.io/LabJournalWebsite/index.html](https://crumplab.github.io/LabJournalWebsite/index.html)

Youtube tutorial: [https://www.youtube.com/watch?v=nc7XhQrasCM&t=1250s&ab_channel=ProgrammingForPsychologists](https://www.youtube.com/watch?v=nc7XhQrasCM&t=1250s&ab_channel=ProgrammingForPsychologists)

Editted for use by Esme Lillywhite for School Attendance project website with Markus Klein and Edward Sosu.

November 2021

# Getting started

*R setup*

* Download and install R and RStudio
* On Rstudio, type into the console:
`install.packages("rmarkdown")`

*GitHub setup*

* Create a github account
* Download GitHub Desktop

# Creating a website from scratch

* First, we create the GitHub repository on github.com using your account.
* Create a repository, and make sure to initialise it with a readme file.
* Once this has been created, open GitHub desktop. Click file, clone repository, and it should show an option for your new repository if you have linked your account. Alternatively, you can use the url of your repository. This can be retreived by going to your repository on github.com, and clicking the code button. Copy and paste the link that appears. Be careful where you clone the repository to- this is where you will add your R project, and it will be difficult to move the file location after this. 
* This should clone your remote repository to your computer. 

* On RStudio, create a new project. Add it to the folder you cloned your repository to. 
* Type into the console `file.create("_site.yml")` This creates the navigation bar that will be the basis of the website
* Type `file.create(“index.Rmd”)` which creates the RMarkdown file for the home page
* These two files will have appeared in the files box in the bottom right hand corner, open both files by double clicking on them
* In the _site.yml_ file, type the following: (directly editting the file, not typing into the console)

```
name: "Schoolattendance"
navbar:
  title: "School Attendance"
  left:
    - text: "Home"
      href: index.html
```
Into the _index.Rmd_ file type:

```
---
title: "Home"
output: html_document
---
```
And then type what you want to appear on your home page. 
* Make sure you save changes to both files, and on the _index.Rmd_ file, click knit.
* This knits the document into a html format, and a window will apear giving you a preview of what you've just created. Make sure you knit before going to the next step.
* In the top right hand box there will be a 'build' tab. Click on this, and then click on 'Build website'. 
* Now you need to push these changes to your remote repository. On GitHub Desktop, the changes you have made should appear on the column at the left handside.
* Type a short summary of your changes, and click commit to master at the bottom.
* The option will appear to push origin. Click this. This pushes your changes to the remote repository.

# Editting this website

* Always fetch origin on GitHub desktop to make sure you have the most uptodate version- pull changes.
* Let others know you're working on changes, so that no ones changes get overridden.
* Open LabJournalWebsite (the RStudio file) to make the changes directly to the web pages.
* Once you've made your changes to the web pages in RStudio, knit the file.
* If you're happy with the preview, click on build website in the build tap on the top right hand box.
* Once this is done, close RStudio, and go to GitHub Desktop.
* On the left hand column, the changes made should automatically be detected.
* Add a short simple summary of changes, and then press commit to origin.
* The option will appear to push origin. Press this. Your changes have now been pushed to the remote repository, and others should be able to see it now.
* Double check it has been successful by going to [https://github.com/esmelillywhite/websiteESRC/](https://github.com/esmelillywhite/websiteESRC/) and checking the changes have appeared. This may take a few minutes.
* After a few minutes, you can also check that the changes went through to the website by clicking the link at the top of this readme file.

Note: Sometimes the update is deleting the CNAME file, and I'm not sure why. If this happens, it can easily be fixed by:
* Go to the settings on the github page for the repo
* Go to pages tab in settings
* Re-add the domain name 'schoolattendance.org'
* This will add the CNAME file. Wait a few minutes and check it's working. 

# Useful Links

[https://www.rstudio.com/resources/cheatsheets/](https://www.rstudio.com/resources/cheatsheets/) Find the Rmarkdown cheat sheet

