<h3>Publish Your Pages <small>Using Github</small></h3>

<ol>
<li>Add a index.html in your project</li>
<li>Create gh-pages branch of this repository</li>
<li>Now go to setting to find : <b><q>your site is published at github_id.github.io/repo_name</q></b></li>
<li>share that link</li>
</ol>
<br/><br/>
<h3>Setting Up git on your Local Machine</h3>

<b>first install</b>
	sudo apt-get install git

<b>configure git</b>
	git config --global user.name "your user name"

	git config --global user.email "email_id"
<b>create a local repository</b>
	git init my_repository
	cd my_repository
	gedit readme
	gedit mycode.c
<b>now add above two files in index.</b>
	git add readme
	git add mycode.c
<b>once we have made all the changes, we commit it</b>
	git commit -m "some_massage"

<b>Now create aa repository on github website</b>
	git remote add origin https:github.com/user_name/my_repository.git
<b>now push files</b>
	git push origin master
	
	
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
