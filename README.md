# Fast git
Bash script that allows you to commit and push to your repository fast.

Often times, when working on small personal projects, we need to quickly add content to the working tree, record the changes and update the remote server.

But typing the git commands can be very repetitive which is why automating can help streamline that process.

### For Mac users

Add to your ``` ~/.bash_profile ``` the following code.


```bash

fastgit() {
	git add .
	git commit -m '$*'
	git push
}
```

Then run ```source ~/.bash_profile```

You can now run in your git folder: ```fastgit "Your commit description" ```

# Fast heroku

Deploy your Heroku applications faster.

First, complete the following tasks:

* Log in your heroku account via SSH. `heroku login`

* Create a new git repository or cd in an existing one.

* Connect to the heroku remote: `heroku git:remote -a YOUR_HEROKU_APP`

### For Mac users


Add to your ``` ~/.bash_profile ``` the following code.


```bash

fastheroku() {
	git add .
	git commit -am '$*'
	git push heroku master
}
```

Then run ```source ~/.bash_profile```

You can now run in your git folder: ```fastheroku "Your commit description" ``` in order to deploy your application.


# Shortcut to popular directory

Add to your ``` ~/.bash_profile ``` the following code.


```bash

popularDir() {
	cd '$PATH'
}
```

Then run ```source ~/.bash_profile```

You can now cd to your popular directory by running `popularDir` from anywhere in your command prompt.
