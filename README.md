# GitHub Instructions
SOPs for the Thelan Tech Github<br>
<img src="https://s-media-cache-ak0.pinimg.com/originals/3c/d5/67/3cd5679f54dc60811383649f9f6ea37d.png"/>
<h2>Overview</h2>
Git is a version control system used to keep track of changes in code which allows multiple people to collaborate on projects and share changes to code seamlessly. It can do a lot, but is very simple. If you are completely new to GitHub I would suggest reading up about what it can do <a href="https://guides.github.com/">here</a>.

<h2>Installing Git</h2>

First off, if you haven't already then you will need to create a GitHub account. You can sign up <a href="https://github.com/">here</a>.

<h3>Windows</h3>
The easiest way to use git on Windows is through their desktop client available <a href="https://desktop.github.com/">here</a>. <a href="https://help.github.com/desktop/guides/getting-started/">Here</a> is a guide on setting it up. The desktop client has a tutorial built into it, but there are also loads of available tutorials and videos online. 

<h3>Mac</h3>
Use the same instructions as above. The desktop client is also available for Mac. 

<h3>Linux</h3>
Most Linux distros already come with git installed. If you're using Linux you probably already know how to use git. If not, there is plenty of good documentation online.  

<h2>Other Requirements</h2>
1. Integrate <a href="www.zenhub.com">ZenHub</a> into your github. Just go to the link and click the big button that says 'Add ZenHub to GitHub' 

<h2>Git Workflow</h2>
*All instructions here are for Windows/Mac users. If you are using Linux then the workflow remains the same, but commands will be issued from the terminal. If you are not familiar with these, consult the github documentation <a href="https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/">here</a>.*
<br><br>
Git has several different workflows. The first is when you are starting a repository for the first time. 

  <h3>Creating a Repository</h3>
  
  Create Repository > Create File(s) > Commit Changes to Master > Sync to Remote Repository
  
  This flow will create a new remote repository which is synced to your local folder. Start by clicking on the plus sign in 
  the top left of the client. You can choose to make a blank repository (Create), clone an existing repository that you have 
  access to (Clone) or initialize git in one that already has files (Add). At the top of the desktop client there are buttons 
  for 'Changes' and 'History'. History shows the timeline of versions etc. for a repo. Changes shows any new files that are 
  not synced with the git repository. By clicking on Changes you are given the choice to 'Commit to master', which will 
  commit the files you have added to the repository.
  
  The second is when you are syncing changes with an existing repo.
  
  <h3>Syncing Changes</h3>
  
  Make Changes > Commit to Branch > Sync with Remote Repository
  
  After making changes to the files in the repository, commit them to the branch you are on (default is master) in the 
  Changes window. You will need to fill in a message to allow you to commit. Once changes are committed, click Sync in
  the top right corner to sync the changes to the repository. This will also pull any changes from the remote repository 
  to your local repository, so be aware of this. This operation should be run at the start of any editing session as well 
  to ensure that you are working on the latest version of any code. 
  
  The third is when you are working on unfinished code that hasn't been tested yet.
  
  <h3>New Branches</h3>
  
  Create New Branch > Make Changes > Commit Changes > Sync > Test > Merge with Master
  
  Arguably the most important part of the workflow. We do not want changes that don't work to be synced with the Master 
  branch, so we use Branches. When you are working on something with other collaborators, but want to commit changes that you 
  are not sure will work so you can keep track of them, then you need to create a new branch. Branches allow you (and others) 
  to experiment on something without having your changes break the Master. You can create a new branch by clicking the 
  'Create new branch' button next to 'master' in the top left. The idea of a branch is that you work in that branch until 
  the changes are either working or prove to be unsuccessful. If they don't work, then discard the branch and return to the 
  master. If they do work, then you 'merge' the branch with the master. You do this by selecting the 'master' branch from the 
  dropdown menu, clicking on 'Compare', selecting the branch that you want to merge into the master, and then clicking 
  'Update from...'. This will merge your changes back into the master branch and end the other branch.  
  
<h2>Warnings & Conventions</h2>

1. NEVER sync changes to the master unless you are sure they work. I mean it. Don't do it. Make a branch and test it, and get someone else to QA it too.
2. For anyone on Linux, never commit without a message. For desktop users it forces you to. Try to be detailed about the reasons for changes and the decision behind using that solution. 
3. Write commit messages in the present tense. Not a massively important one, but it is standard practice. Detailed descriptions can be in past tense. 
4. Always comment your code. Working collaboratively means needing to know what is going on in each other's heads. You can never be too detailed. 
5. Feel free to add your own changes to this doc. That's the whole point of git :) 


  
  
