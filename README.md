- [X] [Rules for Writing md](https://ourcodeworld.com/articles/read/162/tips-and-tricks-that-you-probably-don-t-know-with-the-github-markdown-in-readme-md-files)
- [X] [list of emojis for markdown :blush:](https://www.webpagefx.com/tools/emoji-cheat-sheet/)

### Publishing Your Pages <small><u>Using Github </u></small>

1. check if git is installed  `git --version` 
1. Create a local repo  `mkdir repoName`
1. initialize this repo git init
1. create first file say index.html `touch index.html`
1. check the status `git status` #it shows that git is aware of the file but it is not added to the repo.
    
##### Tracked and Untracked file
* **Tracked** - files that Git knows about and are added to the repository
* **Untracked** - files that are in your working directory, but not added to the repository`
	
##### Git staging environment
> Staged files are files that are ready to be committed to the repository you are working on. <br/>
`git add file_name`
>

##### Git Commit
>Git considers each commit change point or "save point". It is a point in the project you can go back to if you find a bug, or want to make a change.<br/>
__Pro Tip :__ Always include a message while commiting file.<br/> 
`git commit -a -m message`<br/>
__-a:__ If file are not staged, it stages the file and commit
__-m:__ It adds a message
##### Git Commit Log 
>`git log`
>
##### Git Help
> * `git command -help` -  See all the available options for the specific command
> * `git help --all` -  See all possible commands

##### Publishing the page
> 1. Add a index.html in your project
> 1. Create gh-pages branch of this repository
> 1. Now go to setting to find : your site is published at **github_id.github.io/repo_name**
> 1. share that link</li>

<h3>Setting Up git on your Local Machine</h3>

<b>first install Git</b><br/>
	```sudo apt-get install git```

<br/><b>configure git</b><br/>
	```git config --global user.name "your_user_name"```<br/>
	```git config --global user.email "email_id"```
	
<br/><b>To check configured user name and user email</b><br/>
	```git config --global user.name ```<br/>
	```git config --global user.email ```<br/>
	<b>Or Use </b><br/>
	```git config --global --list ```<br/>
	
		   
<br/><b>create a local repository</b><br/>
	```git init my_repository```<br/>
	```cd my_repository```<br/>
	```gedit readme```<br/>
	```gedit mycode.c```
	
<br/><b>now add above two files in index.</b><br/>
	```git add readme```<br/>
	```git add mycode.c```
	
<br/><b>once we have made all the changes, we commit it</b><br/>
	```git commit -m "some_massage"```

<br/><b>Now create a repository on github website</b><br/>

<br/><b>Add origin in your local repository</b><br/>
	```git remote add origin https:github.com/user_name/my_repository.git```
	
<b><br/>Now push files</b><br/>
	```git push origin master```
	
	
<br/>
<h3> Resolving Issues </h3><br/>

 If on adding remote origin gives following error<br/>
   ```raghvendra@raghs-pc:~/raghsgit$ git remote add origin https://github.com/raghsgit/raghsgit.git```<br/>
   ```fatal: remote origin already exists.```<br/>
   
 Resolving<br/>
	```raghvendra@raghs-pc:~/raghsgit$ git remote rm origin```

<br/><b>Download a Project On your system to start work locally</b>
1) Download the repository with its content<br/>
```git clone "<url of project>"```<br/>
2) now edit the files
3) Now add (prepare) files to upload.<br/> 
	```git add *```<br/>
4) if there is a problem in adding files, one solution is to add file forcefully
	```git add -f *```
		
4) Commit the changes, with a message.
	```git commit -m "message"```
5) Upload your file to server
	```git push origin master```



<b>To synchronize with local repository</b><br/>
   1) Add origin master if not added already<br/>
	```git remote add orign https://githubs.com/raghsgit/raghsgit.git```
	
   2) Now Pull the code from server<br/>
	```git pull origin master```
	
   3) to remove origin master<br/>
	```git remote rm origin```

<h3> some Other useful Command</h3>


```git clone url
git remote -v
git remote add upstream
git remote -v

git fetch upstream
git fetch --all
git checkout master
git checkout gh-pages
git merge upstream/master
```

git fetch 
create new branch
git checkout -b <branch_name>
or to switch a branch
git checkout <branch_name>
to merge in header branch=>
git merge origin/<branch_name>





*******************************

# Markdown syntax guide

## Headers

# This is a Heading h1
## This is a Heading h2 
###### This is a Heading h6

## Emphasis

*This text will be italic*  
_This will also be italic_

**This text will be bold**  
__This will also be bold__

_You **can** combine them_

## Lists

### Unordered

* Item 1
* Item 2
* Item 2a
* Item 2b

### Ordered

1. Item 1
1. Item 2
1. Item 3
  1. Item 3a
  1. Item 3b

## Images

![This is a alt text.](/image/sample.png "This is a sample image.")

## Links

You may be using [Markdown Live Preview](https://markdownlivepreview.com/).

## Blockquotes

> Markdown is a lightweight markup language with plain-text-formatting syntax, created in 2004 by John Gruber with Aaron Swartz.
>
>> Markdown is often used to format readme files, for writing messages in online discussion forums, and to create rich text using a plain text editor.

## Tables

| Left columns  | Right columns |
| ------------- |:-------------:|
| left foo      | right foo     |
| left bar      | right bar     |
| left baz      | right baz     |

## Blocks of code

```
let message = 'Hello world';
alert(message);
```

## Inline code

This web site is using `markedjs/marked`.
