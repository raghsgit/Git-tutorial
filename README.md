<h3>Publish Your Pages <small>Using Github </small></h3>

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
	```git config --global user.name "your_user_name"```

	```git config --global user.email "email_id"```
<br/><b>create a local repository</b><br/>
	```git init my_repository<br/>
	cd my_repository<br/>
	gedit readme<br/>
	gedit mycode.c```
<br/><b>now add above two files in index.</b><br/>
	```git add readme<br/>
	git add mycode.c<br/>```
<br/><b>once we have made all the changes, we commit it</b><br/>
	```git commit -m "some_massage"```

<br/><b>Now create a repository on github website</b><br/><br/>
<br/><b>Add origin in your local repository</b><br/>
	```git remote add origin https:github.com/user_name/my_repository.git```
<b><br/>Now push files</b><br/>
	```git push origin master```
	
	
<br/><h3>Resolving Issues </h3>

raghvendra@raghs-pc:~/raghsgit$ git remote add origin https://github.com/raghsgit/raghsgit.git
fatal: remote origin already exists.

do=>
raghvendra@raghs-pc:~/raghsgit$ git remote rm origin
	
// on system to download the project
1) git clone "link"
2) now edit the files
3) git add * (it prepares file to upload not upload)
		if there is a problem one solution is to add file forcefully
	git add -f *
		
4) git commit -m "message" (it also a step before uploading )
5) git push origin master (it pushes the file)



//to synchronize with local repository
first add origin master

git remote add orign https://githubs.com/raghsgit/raghsgit.git
git pull origin master

//to remove origin master

git remote rm origin
