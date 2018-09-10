# fastgit
Bash script that allows you to commit and push to your repository fast.

Often times, when working on small personal projects, we need to quickly add content to the working tree, record the changes and update the remote server.

But typing the git commands can be very repetitive which is why automating can help streamline that process.

## For Mac users

Add to your ``` ~/.bash_profile ``` the following code.


```bash

fastgit() {
	git add .
	git commit '$*'
	git push
}
```

Then run ```source ~/.bash_profile```

You can now run in your git folder: ```fastgit "Your commit" ```
