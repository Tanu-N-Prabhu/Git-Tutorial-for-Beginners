# Git Tutorial for Beginners

## Master Version Control


<!-- Feature Image along with Captions -->
| ![space-1.jpg](https://camo.githubusercontent.com/6eaaae8defc78f268eaf0824350a66a1dfcb6aa77210d3dca069d1d1cefebc53/68747470733a2f2f6769742d73636d2e636f6d2f696d616765732f6c6f676f732f646f776e6c6f6164732f4769742d4c6f676f2d32436f6c6f722e706e67) | 
|:--:| 
| Image Credits - [Jenkins Plugin](https://www.google.com/url?sa=i&url=https%3A%2F%2Fplugins.jenkins.io%2Fgit%2F&psig=AOvVaw01bdtUwTVbMxfTP0Hhog1R&ust=1613868406603000&source=images&cd=vfe&ved=0CAMQjB1qFwoTCODo7rqe9-4CFQAAAAAdAAAAABAD) |


---

# Table of contents
1. [Introduction](#introduction)
    1. [Why Version Control System?](#why)
    2. [Version Control Requirements](#version)
    3. [Two Strategies of Version Control Systems](#two)
        1. [Lock - Modify - Unlock Strategy](#lock)
        2. [Copy - Modify - Merge Strategy](#copy)
    4. [Version Control Systems Handling History](#version1)
        1. [Git](#git)
        2. [Download](#download)

2. [Basic Operations](#basic)
    1. [Creating a GitHub Repository and Clone it](#create)
    2. [Pull Data from the Remote](#pull)

---

# Introduction <a name="introduction"></a>

## Why Version Control System? <a name="why"></a>

Suppose you are working on a simple HTML project, suddenly your boss tells you to change the title of the project. Now you have another version, after that someone else comes and tells you to change the title. This keeps happening for a long time. Now in your system, you have several updated HTML files with new titles. This was the traditional way that the developer used to follow back in the day, where one cannot view what were the changes, and who changed them. This was a problem in those days, but with the help of version control systems, you can easily get the above information without having to save billions of different files in your system.

## Version Control Requirements <a name="version"></a>


* Backup and Restore
* Synchronization
* Undo
* Track Changes and Ownership
* Sandboxing 
* Branching

> **Sandboxing** - Place where you can put all your sample code you don’t need to be published, just like prototyping.

## Two Strategies of Version Control Systems <a name = "two"></a>

* Lock - Modify - Unlock Strategy
* Copy - Modify - Merge Strategy

### Lock - Modify - Unlock Strategy <a name = "lock"></a>


| ![space-1.jpg](https://github.com/Tanu-N-Prabhu/Git-Tutorial-for-Beginners/blob/main/Img/Lock-Modify-Unlock-Strategy.PNG) | 
|:--:| 
| Lock - Modify - Unlock Strategy |


### Copy - Modify - Merge Strategy <a name = "copy"></a>

| ![space-1.jpg](https://github.com/Tanu-N-Prabhu/Git-Tutorial-for-Beginners/blob/main/Img/Copy-Modify-Merge-Strategy.PNG) | 
|:--:| 
| Copy - Modify - Merge Strategy |


Here, Jyothi (developer 2) can resolve the conflict
* Remove her own changes and leave the last one.
* Take some part of her implementation and then push the latest version to the server.


## Version Control Systems Handling History <a name = "version1"></a>

| ![space-1.jpg](https://miro.medium.com/max/3396/1*GgaGcwh5L246YcU5NVDA5A.png) | 
|:--:| 
| Image Credits - [Medium](https://www.google.com/url?sa=i&url=https%3A%2F%2Fmedium.com%2Ffaun%2Fcentralized-vs-distributed-version-control-systems-a135091299f0&psig=AOvVaw1bXx2FflZO4sbmlAhcOotN&ust=1613869347545000&source=images&cd=vfe&ved=0CAMQjB1qFwoTCNC7__uh9-4CFQAAAAAdAAAAABAD) |

> Disadvantage if the entire history is saved in the main server, we need to create some backups




| ![space-1.jpg](https://miro.medium.com/max/1838/1*gPBljo_uRh-IBtHY2oB7ig.png) | 
|:--:| 
| Image Credits - [Medium](https://www.google.com/url?sa=i&url=https%3A%2F%2Fmedium.com%2Ffaun%2Fcentralized-vs-distributed-version-control-systems-a135091299f0&psig=AOvVaw1bXx2FflZO4sbmlAhcOotN&ust=1613869347545000&source=images&cd=vfe&ved=0CAMQjB1qFwoTCNC7__uh9-4CFQAAAAAdAAAAABAD) |


> Each developer has a copy of their own repository, and he/she knows what was changed by who and what. If something happens, then we can use an individual repository as backup.



### Git <a name = "git"></a>

One of the popular Version Control Systems. Please read the [docs](https://git-scm.com/doc)




| ![space-1.jpg](https://github.com/Tanu-N-Prabhu/Git-Tutorial-for-Beginners/blob/main/Img/survey.PNG) | 
|:--:| 
| Image Credits - [Stack Overflow](https://insights.stackoverflow.com/survey/2018#development-practices) |


### [Dowload](https://git-scm.com/downloads) here <a name = "download"></a>

After downloading you can check for the version in your command prompt

```git
git --version

>> git version 2.30.0.windows.2

```

---

# Basic Operations <a name="basic"></a>

## Creating a GitHub Repository and Clone it <a name="create"></a>
1. Go to [GitHub](https://github.com/) and create a new repository with a name **Git-Tutorial-For-Beginners**
    1. Make it **Public**
    2. Include a **README.md** file (enable this option).

2. **Clone** the repository to your system. I personally use Visual Studio Code Terminal. You can use the evergreen Commmand Prompt Termial as well.
    1. Get the clone link from the dropdown which says (Clone or Download).
    2. Type `git clone paste_the_link`.
    3. **Extra Material** - [How to clone a github repository](https://www.youtube.com/watch?v=5RTHaVvj97I)

3. To view the connections of your repository type in `git remote -v`.
4. You can check the status of your repository using `git status`.
5. You can add a new file using `git add index.html`. But the easy way to do it is to create a new html file in your Visual Studio code and then commit to your repository. 
6. To commit, use `git commit -m “message”` will only commit the changes locally.
7. When you refresh your GitHub you won’t see any changes, because you need to **push** the changes to the remote server.
8. To view the log use `git log`.
9. To push use `git push` or sometimes you can use `git push -u origin master` to push the changes.
10. Now when you **refresh** the GitHub repository you can view the changes.


## Pull Data from the Remote <a name="pull"></a>

1. Just make some changes in your initial file ( Main Repository)
2. But in your local system these changes will not be reflected so you need to pull the change (repository) first. Make sure you do this when you are working on a larger project.
3. To pull the change you can use `git pull origin master`.


---

















