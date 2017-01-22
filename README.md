# Sanchittechnogeek.github.io
##### This is my personal blogging website hosted on:

[![N|Solid](https://0ebdc219a6018a0b4949-5cd5d2f3f64eaf0eb4e05aee819f5378.ssl.cf5.rackcdn.com/workflows/deploy-to-github-pages/cover-deploy-to-github-pages.png)](https://pages.github.com/)

You can visit this website for if you are a developer and need help in starting with the following:

  - Open Source development
  - Javascript (inc. MEAN Stack)
  - Fossasia
  - Paas (platform as a service)
  - Docker
  - Penetration testing
  - Google summer of Code
  - Google Code-in

You can also:
  - Clone this repository if you want to setup up your own blogging website using my theme
  - Ping me if you need help in getting started with something
  - etc.

If you like my blogging website and want to host your own but don't know how to use Git and Github. I'll help you to get started by:

- how to clone my repository
- how to upload it to gh-pages

###### Note: You will be learning some basic git commands along the way

### Tech Stack

I am using :

* JavaScript - commonly used to create interactive effects within web browsers.
* Twitter Bootstrap - great UI boilerplate for modern websites
* CSS - Serving html content beautifully
* jQuery - a javascript library for handling animation etc.

And of course my website itself is open source with a public repository on GitHub.

## If you are a beginner and unfamiliar with Git and Github:

### Installation

[Git bash](https://git-scm.com/download/win) (windows) or Git cli (ubuntu/linux) along with an account on [GitHub](https://github.com/join) is required to get started.

As we are familiar with using Ubuntu, all we got to do is, open the terminal and type the following:
```sh
$ sudo apt-get install git-core git-gui git-doc
```
It’s your call, if you want to get the Git docs as well. Else the git-core files would be just enough.

### Setting up the SSH key on our system

Now, we need to generate a SSH key for your system. It’s as easy as opening a terminal and typing ‘ssh-keygen‘ and then pressing enter. Follow the further instructions and you get the SSH key generated under the .ssh/id_rsa.pub file. No worries, the full path of the file shows up as soon as the SSH key gets generated.

### Add your SSH key to GitHub
###### NOTE: This is not necessary. If you want you can skip this step

The next step is to paste the generated SSH key to the corresponding textarea on the Git profile page. So, proceeding step-wise,
1. Open the generated id_rsa.pub file on your system and copy all of its content.
2. Login to Git.
3. Go to your profile update page. You can see the textarea for ‘Add a public key’.
4. Paste the content you copied in Step 1 to the textarea you focussed in Step 3
5. Click on ‘Update your account‘ button and done!

### Setting up the user info

Next, we need to enter the user details. Most importantly the username and the email. It has a significance though, as to why they are the most important.  If there are 20 people involved on a single project, all the changes done by each of them are intimidated to all the people involved on that project. So we get a clear notification if a certain user has made certain changes to some file. Now, to update the username and the email, type the following in the terminal window:
```sh
git config --global user.name "your name here"
git config --global user.email abc@test.com
```
We can check the status anytime by typing:

```sh
git config --list
```
So, we are done with all the minimal configuration needed to start committing and pushing your codes. Also do remember, this is a one time setup and doesn’t need to done everytime we start with a new project.
##### Now as everything is nice, sweet. we can start to clone our repository

### Cloning the repository
open the terminal and type:
```sh
$ git clone https://github.com/sanchittechnogeek/sanchittechnogeek.github.io.git
```

After the repository has been clone, Head over to GitHub and create a new repository named username.github.io, where username is your username (or organization name) on GitHub.
###### Note: If the first part of the repository doesn’t exactly match your username, it won’t work, so make sure to get it right.
#
When you clone a repository, it is added as a remote of yours, under the name origin. or simply The repository you have cloned comes with the original origin URL. What you need to do now (as you're not using the old source anymore) is change origin's URL:

```sh
$ git remote set-url origin http://github.com/username/username.github.io
```
###### Note: Make sure your replace 'username' with your github username.
#
>Now you are free to make changes to the repository/files.


### Adding files to the staging area and committing them

Open your terminal and cd into the repository/the website's folder. After getting into the repository , you have to add the new changes to the files to the staging area. so lets do it:
```sh
$ git add .
```
by typing [.] istead of the file name will add all the changes the files to the staging area. Now you are ready to commit, but lets check status before that by typing:
```sh
$ git status
```
It will show you that the files are ready to be committed. So lets commit them by writing a simple commit message using the [-m] flag:
```sh
$ git commit -m "Your commit message"
```
Now you are ready to push the change to your repository, but lets check status before that by typing:
```sh
$ git status
```
It will show you something like no files are needed to be committed.
As everything is nice and sweet here, lets check if our commit actually worked by typing:
```sh
$ git log
```
Now it will show you something like 088c08u00c... with a commit message , time, date and with account info.

>After you are done , now its time to push it to your gh-pages repository

### Pushing the files to your Github Pages repository

Now to push your files to Github Pages repository, type:
```sh
$ git push origin master
```
It will now ask you for your github username and password for confirmation, enter it then press enter and Wala! , You will see a message stating all the files has been pushed to your repository's master branch.

### Now you have your blogging site up and running at: https://username.github.io
