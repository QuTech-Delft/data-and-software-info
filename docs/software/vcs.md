# Version Control Systems

This page gives some information about version control systems. If you are already familiar with those you might want to skip ahead to see if the additional resources offer something new to learn for you. On this page we give a short description of the version control infrastructure available to researches at QuTech. If version control systems are new for you then we will begin by explaining which problems they can help solve, how they do this and what tools you can use for this.

## Why?

If you have previously developed code you might have experienced some of the following problems:

* Something that previously worked is suddenly broken. It takes a long time to bring it back to a working state.
* You have accidentally deleted some code, the laptop with your precious code on it was stolen or you have lost code in some other way.
* You want to collaborate on code, but it is not easy to work on the same project at the same time with your colleagues.
* You or someone else wants to reproduce results you have obtained in the past, but you have changed the code and the results have changed.

Version control systems have been created to tackle exactly these types of problems when developing software. How they do that and which systems are available for it in QuTech will be explained next.

## How?

Version control systems work with a local version and a remote version of your code. The place where your code is stored is called a repository. Each developer can start working in a local repository on their own computer. Once they are finished making changes they upload (called push) their local repository to synchronize it with the remote repository. In this way your code is always backed up in a remote location. Since it is backed up on a server you can also use this remote copy to share your code with others or to collaborate on the code.

The version control systems, as the name implies, also has a form of versioning. When new code is pushed to the remote repository the system does more than just saving this latest version. The system keeps track of the changes that have been made in the past and therefore also allows you to look through the history of your code and to retrieve old versions. This has several advantages. You can change your code without being scared of breaking it, you can always go back to a working version. You can easily use and share old versions of your code to reproduce old results. You can figure out when something changed, who changed it and why it was changed.

Additionally version control systems have a concept called branches, which allows for more advanced collaboration. If you just want to use version control systems as a solo developer you probably do not need to think about this. We briefly cover the topic of branches here though: Branches allow you to “branch off”. When you do this you create a new copy of your code which is stored separately from your main code (stored on the main branch). You can then start making changes on this branch and once you are finished you can add the changes you have made back your main branch, incorporating them into your “normal” code. This allows for more collaboration on the same codebase. Different features for example can be worked on simultaneously on different branches.

There are different philosophies about how you can use these branches to collaborate, each having their own advantages and disadvantages. We will give some more information on these different workflows in the additional resources. If you are unsure how best work with the branches for your project you can also ask the SDST for advice.

## What?

There are different version control systems. At QuTech mostly **Git** is used, this is also one of the most popular version control systems. The additional resources section provides information on learning Git if you are not yet familiar with it. If you are familiar it also offers some advanced topics if you want to learn more.

As mentioned version control systems store your code remotely. This means that next to a system such as Git you also need a server to store the code on. There are a few options for this. The two most popular options are GitHub and GitLab. At QuTech we also have the possibility to use a version of GitLab hosted by the TU Delft. Your research group might already have a preferred option so you might want to ask your supervisor what is used in your group. If your research group does not have a preferred option yet you can ask the SDST for help with selecting one.

### Additional Resources

Interested in version control systems, but unsure how to continue from here? You can always ask the SDST for help/advice on this topic. Additionally if you want to learn more about Git we provide some resources for you here.

#### All Levels

* Need a reminder of the commands used in Git? GitHub has a convenient [cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf):
* Would you rather use a GUI instead of (or in combination with) command line commands? A few different GUIs are availabe, some examples:
  * [Sourcetree](https://www.sourcetreeapp.com/):
    * Free and popular GUI with a lot of features
  * [Fork](https://git-fork.com/)
    * Free at the moment, most likely will cost some money in the future
  * [GitHub Desktop](https://desktop.github.com/)
    * Free. Generally easy to use, but tailored to GitHub specifically

#### Beginners

Want to learn the basics of Git?

* The TU Delft library offers three different courses which teach you about Git (and give you graduate school credits!)
  * (1.5 GS credits) A [course about Git](https://www.tudelft.nl/library/research-data-management/r/training-evenementen/training-voor-onderzoekers/version-control-collaborative-development-for-research-software)
  * (2.5 GS credits) A [more general course](https://www.tudelft.nl/library/research-data-management/r/training-evenementen/training-voor-onderzoekers/coderefinery-workshops) to refine your coding skills, which includes an introduction to Git
  * (1.5 GS credits) A [programming introduction course](https://www.tudelft.nl/library/research-data-management/r/training-evenementen/training-voor-onderzoekers/software-carpentry-workshops) for researches with little to no experience with programming, which includes an introduction to Git
* Would you rather learn more about Git at your own pace?
  * [This short freecodecamp tutorial](https://www.freecodecamp.org/news/introduction-to-git-and-github/) explains how to get started with Git and GitHub
  * Want to learn Git while sovling puzzles? [This interactive game](https://learngitbranching.js.org/) teaches you about Git commands (you might need to disable your adblocker if you have one for it to work properly)

#### Intermediate/Advanced

* Do you know the basics, but want to know more about workflows to use Git to collaborate?
  * GitLab has [an overview of some different workflows](https://about.gitlab.com/topics/version-control/what-is-git-workflow/) and their advantages:  
  * In [this article](https://www.atlassian.com/git/tutorials/comparing-workflows) Atlassian describes the basic “Centralized Workflow” and links to elaborate descriptions of other workflows
