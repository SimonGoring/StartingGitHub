StartingGitHub
==============

This repository is associated with, and modified from, a [post](http://downwithtime.wordpress.com/2013/09/12/writing-and-collaborating-on-github-a-primer-for-paleoecologists/) by Simon Goring at [downwithtime](http://downwithtime.wordpress.com) teaching people how to get started using [GitHub](http://github.com).

Contributors
----------------
Simon Goring
Julia Barthold
Jess Tauber


Introduction
------------------------
At this point I've written a hundred times about the supplement for Goring et al., (2013), but just in case you haven't heard it:

Goring et al., ([2013](http://onlinelibrary.wiley.com/doi/10.1111/1365-2745.12135/full)) uses a large vegetation dataset to test whether or not pollen richness is related to plant richness at a regional scale. Because of the nature of the data and analysis, and because I do all of my work (or most of it) using R, I thought it would be a good idea to produce totally reproducible research.  To achieve this I included a version of the paper, written using [RMarkdown](http://www.rstudio.com/ide/docs/authoring/using_markdown), as a supplement to the paper.  In addition to this, I posted the supplement to [GitHub](http://github.com) ([here](https://github.com/SimonGoring/GoringetalPollenRichness)) so that people who were interested in looking at the code more deeply could create their own versions of the data and could use the strengths of the GitHub platform to help them write their own code, or do similar analyses.

This is a basic how-to to get you started writing your paper using RMarkdown, RStudio and GitHub (EDIT: if some of these instructions don't work let me know and I'll fix them immediately):

Installing Programs
----------------------------------
* If you don't already, install [RStudio](http://www.rstudio.com/).  There's lots of other development platforms for R, and some of them do have integration with GitHub (this [notepad++](http://notepad-plus-plus.org/) [plugin](https://forum.lowyat.net/topic/1358320/all) for example), but I haven't tried them so I can't recommend them.

* Sign up for a GitHub account ([here](https://github.com/signup/free)) and install both the GitHub GUI ([Windows](http://windows.github.com/), [Mac](http://mac.github.com/), Linux users are probably well beyond this point already) and [Git](http://git-scm.com/).

Finding a Project
----------------------------------
* Now you need a project.  I've created a project on GitHub called "[StartingGitHub](https://github.com/SimonGoring/StartingGitHub)", that is going to support a tutorial to help people get started with GitHub, and everyone is welcome to join in and build it.   The first thing you need to do is go to my repository and [fork it](https://help.github.com/articles/fork-a-repo).  This will create your own personal version of the project in your own personal space on GitHub.  Once you've forked the repository open up the GitHub GUI.

* Open the GitHub GUI.  You should see something that looks like Figure 1.  This shows that I have some local copies of my GitHub repositories, and that I have my own web repository, and I am a member of the ropensci organization.

![Figure1][Figure1_image]

**Figure 1**. *When you open up the GitHub GUI you should see the repositories you are associated with (Column 1), local repositories (Column 2) and the contents of readme files for any selected repositories (Column 3).*

* Click on your user name under "GitHub". You should see the repository you've just forked, "Starting GitHub".  When you click on it you'll see text appear in the third column, this is the readme file.  Now clone it by clicking the word "CLONE", this will put a copy of the repository into a directory in your GitHub folder.

![Figure2][Figure2_image]

**Figure 2**.  *You should see a tab called "Git" in your workspace pane (top right pane in the RStudio window).*

Creating & Editing a Version Controlled Project
-----------------------------------------
* Open up RStudio (if it's been open this whole time, close it and open it again).  You're about to create a project.  Click the "Project" menu, "Create Project" and then link it to an "Existing Directory".  Because you've cloned it RStudio knows that this file is associated with a GitHub account, so that when the project is opened you should have a tab in your workspace window that says "Git" (Figure 2).

* Now you're ready to edit.  Open the file "README.md".  This file is the file you see in the GitHub GUI when you click on "StartingGitHub".  You're almost finished with your first edit, so just add your name to the file under the "Contributors" heading.

* Save the file, and you should see the file "README.md" appear under the Git tab in the top right of your RStudio window.  This means that you have made a change to the file, so click on the word "Diff" (right under "Workspace", above "Staged") and you'll see a new window appear that will highlight your changes in red (text you've deleted) and green (text you've added).  If you've just added your name then that should appear in green.

* So that looks good so far, click the box beside the filename (under "Staged", this means we're going to accept the changes, now type in a message in the box labeled "Commit message", something clear and descriptive ("Added my name to the list of contributors"), and then click commit.

* Okay, you should have seen a new, little black window appear, close that, and then lets send the change to the web (it's only on your computer right now).  You want to click the "Push" button here (top right in the "Diff" window that we just entered our commit message in), enter your github user name and password when prompted.  And voila!  There you go!  The change has been pushed to your repository.

Your Progress So Far (Great!)
-----------------------------------
So what have you done:
* You downloaded all the programs
* You created a GitHub user account
* You forked and cloned a repository
* You created a version controlled R Project
* You made a minor edit, committed the change and then pushed it back up to your GitHub account.
* You are awesome!

*But wait!*  That change was really good, and it should be part of the main repository so everyone else can see it.  You're going to need to Push your changes.

Pushing Change
--------------------
* Go back to your GitHub account online and open up the repository.  You'll see all the file names in the repository and the notes associated with their last commit.  You'll also see a green box with some arrows, that will let you push your changes back to the parent repository, my StartingGitHub repository.  

* When you click the green box you should see your commit message, the changes you made, and, beside your avatar, text that says "Click to create a pull request for this comparison".  Click this button, if you want to amend your commit message you can now (you don't have to) and then click "Send Pull Request".

* Now it's all up to me to decide whether I want to include your change or not, but you're done!  

**Congratulations, you're off to the races.**

[Figure1_image]: figures/GitHub_GUI_screenshot.png "screenshot"
[Figure2_image]: figures/GitInPane.png "GitPane"