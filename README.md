<h3>Publishing Your Pages <small>Using Github </small></h3>

<ol>
<li>Add a index.html in your project</li>
<li>Create gh-pages branch of this repository</li>
<li>Now go to setting to find : <b><q>your site is published at github_id.github.io/repo_name</q></b></li>
<li>share that link</li>
</ol>
<br/><br/>
<h3>Setting Up git on your Local Machine</h3>

<b>first install Git</b><br/>
	```sudo apt-get install git```

<br/><b>configure git</b><br/>
	```git config --global user.name "your_user_name"```<br/>
	```git config --global user.email "email_id"```
	   
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

1) If on adding remote origin gives following error<b/><br/>
   ```raghvendra@raghs-pc:~/raghsgit$ git remote add origin https://github.com/raghsgit/raghsgit.git```<br/>
   ```fatal: remote origin already exists.```
2) Resolving
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

