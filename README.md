[![](https://img.shields.io/badge/github-blue?style=for-the-badge)](https://github.com/hamzamohdzubair/redant)
# **$${\color{Indigo}Welcome \space To \space Github \space!!}$$**                                                            

This repo gives a brief description about github and how to work with github, along with some hands-on.

## Please follow the link below to Open a blank issue in the welcome repo to get started 

🔗 https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue

> 🚩 **Note: Open a Issue with the title "Github hands-on"**

<br>

### 💡 **What Is GitHub? A Beginner’s Introduction to GitHub**

At a high level, GitHub is a website and cloud-based service that helps developers store and manage their code, as well as track and control changes to their code. To understand exactly what GitHub is, you need to know two connected principles:

- Version control                   
- Git                         

<p align="center">
  <img src="https://github.com/eidikodev/Git-Best-Practices/blob/test-update--5/centralized-vs-distributed.jpg" width=50% height=50%/>
</p>

### 💡 What Is Version Control?

Version control helps developers track and manage changes to a software project’s code. As a software project grows, version control becomes essential.This is a centralized way, there will be a single source or a central copy of your repository. You’ll have to grant permission to other team members/ add them as contributors to this central repositories(Central repositories are a matter of project organization), for them to start contributing to your central repo.version control lets developers safely work through branching and merging.

With branching, a developer duplicates part of the source code (called the repository). The developer can then safely make changes to that part of the code without affecting the rest of the project.Then, once the developer gets his or her part of the code working properly, he or she can merge that code back into the main source code to make it official.

All of these changes are then tracked and can be reverted if need be.

### 💡 What Is Git?

Git is a free and open-source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.Git is a distributed version control system, which means that the entire codebase and history is available on every developer’s computer, which allows for easy branching and merging.

<p align="center">
  <img src="https://github.com/eidikodev/Git-Best-Practices/blob/test-update--5/distributed-1024x677.png" width=50% height=50%/>
</p>

 ***

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#Setting-up-Git-in-your-local">Setting-up-Git-in-your-local</a>
      <ul>
        <li><a href="#To-configure-user-information-for-all-local-repositories">To configure user information for all local repositories</a></li>
        <li><a href="#Authenticating-with-GitHub-from-Git">Authenticating with GitHub from Git</a></li>
        <li><a href="#Creating-a-personal-access-token">Creating a personal access token</a></li>
        <li><a href="#Generating-a-new-SSH-key-and-adding-it-to-the-ssh-agent">Generating a new SSH key and adding it to the ssh-agent</a></li>
        <!-- <li><a href="#built-with">Built With</a></li> -->
      </ul>
    </li>
	<!-- <li><a href="#How-To-Use-Git-And-GitHub-At-Kellogg">How To Use Git And GitHub At Kellogg</a>
</li> -->
<!--    </ul>-->
      <li>
	<a href="#Get-Started-Learning-GitHub">Get Started Learning GitHub</a>
      <ul>
        <li><a href="#GitHub Introduction">GitHub Introduction</a></li>
        <li><a href="#Merge-conflicts">Merge conflicts</a></li>
        <li><a href="#Git-Actions">Git Actions</a></li>
        <!-- <li><a href="#built-with">Built With</a></li> -->
      </ul>
    </li> 
	  <li>
		  <a href="#GitHub-best-practices">GitHub best practices</a>
      <ul>
          <ul><li><a href="#Who-this-guide-is-for">Who this guide is for</a></li></ul>
		  <ol type=1><li><a href="#Do-not-git-push-straight-to-master">Do not git push straight to master</a></li>
          <li><a href="#Do-not-commit-code-as-an-unrecognized author">Do not commit code as an unrecognized author</a></li>
          <li><a href="#Define-code-owners-for-faster-code-reviews">Define code owners for faster code reviews</a></li>
          <li><a href="#Do-not-leak-secrets-into-source-control">Do not leak secrets into source control</a></li>
          <li><a href="#Do-not-commit-dependencies-into-source-control">Do not commit dependencies into source control</a></li>
          <li><a href="#Do-not-commit-local-config-files-into-source-control">Do not commit local config files into source control</a></li>
          <li><a href="#Create-a-meaningful-git-ignore-file">Create a meaningful git ignore file</a></li>
          <li><a href="#Archive-dead-repositories">Archive dead repositories</a></li>
          <li><a href="#Lock-package-version">Lock package version</a></li>
          <li><a href="#Specify-standard-package-versions">Specify standard package versions</a></li>
          <li><a href="#Leverage-task-list">Leverage task list</a></li>
          <li><a href="#Use-a-branch-naming-convention">Use a branch naming convention</a></li>
          <li><a href="#Delete-stale-branches">Delete stale branches</a></li>
          <li><a href="#Keep-branches-up-to-date">Keep branches up to date</a></li>
          <li><a href="#Remove-inactive-GitHub-members">Remove-inactive-GitHub-members</a></li>
          <li><a href="#Enable-security-alerts">Enable security alerts</a></li>
      </ul>
    </li>   
 
 <li>
      <a href="#Issues">Issues</a>
  </li>
 
 <li>
      <a href="#Other-Git-and-GitHub-learning-resources">Other Git and GitHub learning resources</a>
    </li>
  <li>
      <a href="#Recommended-GitHub-Actions">Recommended GitHub Actions</a>
  </li>
    
   <li>
      <a href="#Glossary">Glossary</a>
  </li>
 </ol>
</details>
	
## 🪁Setting up Git in your local
To set git locally, install **GitBash** or **GitHub-desktop** 

A new repository can either be created locally, or an existing repository can be cloned. When a repository was initialized locally, you have to push it to GitHub afterwards.

<br>
<br>

using GitBash(CLI) or GitHub-Desktop(GUI),run the following commands 

🖍️ **```git init```**

  The git init command turns an existing directory into a new Git repository inside the folder you are running this command.
         

### To configure user information for all local repositories,Run the below commands

🖍️ **```git config --global user.name "[FIRST_NAME LAST_NAME]"```**

  Sets the name you want attached to your commit transactions

🖍️ **```git config --global user.email "[MY_NAME@kellogg.com]"```**    

  Sets the email you want attached to your commit transactions
    

🖍️ To Set/Check proxy

  **```git config --global --add remote.origin.proxy "127.0.0.1:9000"```**  

  To add Proxy details to Git Bash to make it Proxy aware: 

  Navigate to Windows -> GitBash 

  Run: “git config --global --add remote.origin.proxy "127.0.0.1:9000"”. 

  To validate and ensure the proxy is listed in the config: 

  Navigate to Windows -> GitBash 

  Run: “git config -l”

🖍️ **```git remote add origin [url]```**

  Specifies the remote repository for your local repository. The url points to a repository on GitHub.
    
🖍️ **```git clone [url]```**

  Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits

<p align="center">
  <img src="https://github.com/eidikodev/Git-Best-Practices/blob/test-update--5/github%20cycle.jpg" width=50% height=50%/>
</p>

<br>

### Authenticating with GitHub from Git
When you connect to a GitHub repository from Git, you will need to authenticate with GitHub using either HTTPS or SSH.

> 🚩 **Note: You can authenticate to GitHub using GitHub CLI, for either HTTP or SSH.**

### Connecting over HTTPS (recommended)
If you clone with HTTPS, you can cache your GitHub credentials in Git using a credential helper. For more information, see 🔗 "[Cloning with HTTPS urls](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls)" and 🔗 "[Caching your GitHub credentials in Git](https://docs.github.com/en/get-started/getting-started-with-git/caching-your-github-credentials-in-git)."

Cloning with HTTPS URLs
The https:// clone URLs are available on all repositories, regardless of visibility. https:// clone URLs work even if you are behind a firewall or proxy.

When you git clone, git fetch, git pull, or git push to a remote repository using HTTPS URLs on the command line, Git will ask for your GitHub username and password. When Git prompts you for your password, enter your personal access token. Alternatively, you can use a credential helper like Git Credential Manager. Password-based authentication for Git has been removed in favor of more secure authentication methods. For more information, see "Creating a personal access token."

### Creating a personal access token

Personal access token are an alternative to using passwords for authentication to GitHub when using the GitHub API or the command line. It is recommanded to use PAT instead of using GitHub user defined password.
Please click the below link to creating a personal access token (PAT) :

🔗 https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token


### Connecting over SSH
If you clone with SSH, you must generate SSH keys on each computer you use to push or pull from GitHub. For more information, see 🔗"[Cloning with SSH urls](https://docs.github.com/en/get-started/getting-started-with-git/about-remote-repositories#cloning-with-ssh-urls)" and "Generating a new SSH key."

### Generating a new SSH key and adding it to the ssh agent

You can access and write data in repositories on GitHub.com using SSH (Secure Shell Protocol).
When you generate an SSH key, you can add a passphrase to further secure the key. Whenever you use the key, you must enter the passphrase. If your key has a passphrase and you don't want to enter the passphrase every time you use the key, you can add your key to the SSH agent. The SSH agent manages your SSH keys and remembers your passphrase.

Please click the below link to generating a new SSH key and adding it to the ssh-agent :

> 🚩 **Note: For any of the kellogg server's, if you would like to establish SSH connection then create SSH Keys to the server**

🔗 https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=windows
<br>

***

## 🪁Get Started Learning GitHub 

> 🚩 **Note: It is recommended to complete the exercise given in the below course**
###  🚩🚩**Note: Use personal Github account for Training Modules instead of kellogg's organization***

### GitHub Introduction

GitHub is a development platform that enables you to host and review code, manage projects, and build software alongside 50 million developers.

Learn to use key GitHub features, including issues, notifications, branches, commits, and pull requests.

Please click the below link to start learning Github.

🔗 https://learn.microsoft.com/en-us/training/modules/introduction-to-github/

### Merge conflicts
When Git cannot perform an auto-merge because changes are in the same region this causes merge conflicts. Many developers are confused about concepts like merging and resolving merge conflicts. Here, we will learn how to resolve merge conflicts. 

🔗 https://learn.microsoft.com/en-us/training/modules/resolve-merge-conflicts-github.

### Github Actions 
Automate, customize, and execute your software development workflows right in your repository with GitHub Actions. You can discover, create, and share actions to perform any job you'd like, including CI/CD, and combine actions in a completely customized workflow.Learn how to use GitHub Actions using below link.

🔗 https://learn.microsoft.com/en-us/training/modules/introduction-to-github-actions/
	  
<br>

> 🛎️🚩 ### **```Please use kellogg's template while you create a repository```** ,Here is the link to learn how to [create repository using template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)

<br>

***
		  
## 🪁GitHub best practices

This list of GitHub best practices is derived from the insights we gleamed from those experiences.These best practices are still applicable even if you use something other than GitHub for source control, because they’re all about improving code quality, security, and writing good code.

 <p align="center">
  <img src="https://github.com/eidikodev/Git-Best-Practices/blob/test-update--5/og-git-best-practices-1024x538.png" width=100% height=30%/>
</p>


### 📰Who this guide is for
This guide is for anyone in the Application development Teams looking to improve developer workflow and productivity, as well as code quality and security.

Those responsible for putting together team-wide standard practices and policies would benefit greatly from this guide, but even if you’re a developer not “in charge” of driving such standards, you will find these practices applicable and useful to remember.
### 🔖Do not git push straight to master

Regardless if you use Gitflow or any other git branching model, it is always a good idea to turn on git branch protection to prevent direct commits and ensure your main branch code is deployable at all times. All commits should be pushed to master through pull requests.


### 🔖Do not commit code as an unrecognized author
Sometimes you commit code using the wrong email address, and as a result GitHub shows that your commit has an unrecognized author. Having commits with unrecognized authors makes it more difficult to track who wrote which part of the code.

Ensure your Git client is configured with the correct email address and linked to your GitHub user. Check your pull requests during code reviews for unrecognized commits.

### 🔖Define code owners for faster code reviews
When you’re dealing with dozens, hundreds, or more repositories and engineers, it’s nearly impossible to know who owns which parts of the codebase and need to review your changes.

Even in smaller teams you’d still have code owners – for example, front-end code changes should be reviewed by the Front-End Engineer.

Use Code Owners feature to define which teams and people are automatically selected as reviewers for the repository.
There is an option for projects where you want to keep more control. A protected branch option means that the code owner for each owned file has to leave a review before anyone can merge a pull request to that branch.

### 🔖Do not leak secrets into source control
Secrets, or secret keys or secret credentials, include things like account passwords, API keys, private tokens, and SSH keys. You should not check them into your source code.Instead, we recommend you inject secrets as environment variables externally from a secure store. You can use tools like Hashicorp Vault or AWS Secrets Manager to do this.

There are also tools for scanning secrets in repos and prevent them from getting into repos.

Git-secrets can help you to identify passwords in your code.Git hooks can be used to build a pre-commit hook and check every pull request for secrets.

### 🔖Do not commit dependencies into source control
Pushing dependencies into your remote origin will increase repository size. Remove any projects dependencies included in your repositories and let your package manager download them in each build. if you are afraid of “dependencies availability” you should consider using a binary repository manager solution like Jfrog or Nexus Repository. Or check out GitHub’s Git-Sizer.

### 🔖Do not commit local config files into source control
We strongly recommend against committing your local config files to version control. Usually, those are private configuration files you don’t want to push to remote because they are holding secrets, personal preferences, history or general information that should stay only in your local environment.

### 🔖Create a meaningful git ignore file
A .gitignore file is a must in each repository to ignore predefined files and directories. It will help you to prevent secret keys, dependencies and many other possible discrepancies in your code. You can choose a relevant template from Gitignore.io to get started quickly.

### 🔖Archive dead repositories
Over time, for various reasons, we find ourselves with unmaintained repositories. Sometimes developers create repos for an ad hoc use case, a POC, or some other reason. Sometimes they inherit repos with old and irrelevant code.

In any case, these repos were left intact. No one is doing any development work in those repos anymore, so you want to clean them up and avoid the risk of other people using them. The best practice is to archive them, i.e. make them “read-only” to everyone.

### 🔖Lock package version
Your manifest file contains information about all packages and dependencies in your project and their versions. The best practice is to specify a version or version range for every package and dependency listed in the manifest. Otherwise, you can’t be sure which version will get installed during the next build, and consequently your code may break.

### 🔖Specify standard package versions
Even when everyone on your team are using the same packages, reusing code and tests across different projects can still be difficult if the packages are of different versions.

If you have a package that is used in multiple projects, try at a minimum to use the same major version of the package.

### 🔖Leverage task list
Tasks lists provide a way for you to track to-dos directly within comments, issues, and even MarkDownfiles (*.MD) within your repository (users must have write access to the repository to make changes to MarkDownfiles).

Tasks lists provide an excellent way to capture a high-level overview of a task or issue, as well as keep others updated on its state. Make sure to take advantage of this powerful new feature!

### 🔖Use a branch naming convention
Adopting a consistent branch naming convention is essential to keeping your repository organized as your team grows in size. An efficient naming convention will allow you to keep merge conflicts at a minimum while ensuring your developers are as productive as possible.

While there are many branch naming conventions, one of the most popular ones is known as git flow:

![Alternative text](https://github.com/eidikodev/Git-Best-Practices/blob/master/git%20flow.png)

### 🔖Delete stale branches
Every time one branch is merged into another, the branch that is merged in becomes stale, assuming further work isn’t being done in it.While it may seem useful or even necessary to keep the extra data on hand, the reality is that stale branches are abandoned 98% of the time and simply clutter up your project.

Even if you delete a branch when you shouldn’t have, you can restore it - and if you don’t trust GitHub’s restore feature,  chances are it’s safe on somebody’s computer, thanks to the magic of distributed versioning.

Don’t be a branch hoarder: delete your stale branches.

### 🔖Keep branches up to date
Let’s say you’ve finally completed some work on a long-outstanding branch and you’re ready to merge it into master. You pull from remote, hit merge, and suddenly you’re faced with a barrage of merge conflicts.

What happened?🤔

You failed to keep your branch up-to-date with the branch you’re attempting to merge into. Lots of commits went by and some conflicted with your changes... now you’re faced with spending time and energy resolving an unnecessary amount merge conflicts.

The best practice here is to ensure that you’re consistently merging your base branch into your current branch as you work, especially if it’s a long-outstanding branch.

### 🔖Remove inactive GitHub members
While it might seem obvious, it’s worth mentioning in a comprehensive list of best practices... Be sure to remove contributors from your organization that are no longer contributing to your codebase.

If you remove somebody from your organization for any reason, revoke their GitHub access immediately as well. Even in completely amicable situations, it’s better safe than sorry!

### 🔖Enable security alerts
Security alerts are another feature new to GitHub. You can read about them here, but the gist is that GitHub now tracks reported security vulnerabilities in some dependencies and will even suggest fixes for you.

This is turned on automatically for all public repositories, but if your repository is private, you’ll need to opt in manually.



***

## 🪁Issues

Issues can be used to keep track of bugs, enhancements, or other requests. For more information, see "🔗[About issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)".

GitHub now also supports 🔗[multiple issue templates](https://help.github.com/articles/about-issue-and-pull-request-templates/). Feel free to log issues.

***
## 🪁Other Git and GitHub learning resources
		  
🔗  [ProGit book](http://git-scm.com/book) 

🔗  [Git docs](https://docs.github.com/en/get-started/using-git/about-git)

🔗  [Git command list](https://git-scm.com/docs)

🔗  [GitHub training & Guides in youtube](https://www.youtube.com/githubguides)
                                                                              		  
***

## 🪁Recommended GitHub Actions

Some starter [GitHub Actions workflows](https://docs.github.com/en/actions/learn-github-actions) included with this repo are:

🔗  [Stale issue](https://github.com/actions/stale) - labels and closes issues and pull requests with no activity for a set period of time

🔗  [LFS Warning](https://github.com/ActionsDesk/lfs-warning) - issues warnings when large files are added to the repository

🔗  [Release Drafter](https://github.com/marketplace/actions/release-drafter) - drafts release notes based on merged pull requests

🔗 [First Interaction](https://github.com/actions/first-interaction) - Greets new contributors to the repo

🔗 A [Dependabot config file](https://docs.github.com/en/github/administering-a-repository/configuration-options-for-dependency-updates) for alerting on dependency vulnerabilities

***
## 🪁Glossary

***git:*** an open source, distributed version-control system

***GitHub:*** a platform for hosting and collaborating on Git repositories

***commit:*** a Git object, a snapshot of your entire repository compressed into a SHA

***branch:*** a lightweight movable pointer to a commit

***clone:*** a local version of a repository, including all commits and branches

***remote:*** a common repository on GitHub that all team members use to exchange their changes

***fork:*** a copy of a repository on GitHub owned by a different user

***pull request:*** a place to compare and discuss the differences introduced on a branch with reviews, comments, integrated tests, and more
