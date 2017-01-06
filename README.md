Battle of the Beards
====================
This is the repo for the [Battle of the Beards](http://battleofthebeards.info) website, which uses [Hugo](http://gohugo.io) a static website engine.

Pull requests are welcome! There are a few ways you can make changes

* You can do it from github, click the edit file to get started
  * this is great for fixing things like typos
* Install Hugo on your machine, make the changes, preview them, commit them and make a pull request
  * this is the best way to make change that might effect the layout

Installing Hugo
---------------
You'll first need to [Install Hugo](http://gohugo.io/overview/installing) in a way that best suits your environment and comfort level.

Using Hugo
----------
In a command prompt or terminal, navigate to the path that contains your `config.toml` file and run `hugo`.
You should now have a `public` directory with a complete blog! Open `public/index.html` in your browser and bask.

Live Editing
------------
If that wasn't amazing enough, from the same terminal, run `hugo server -w`. This will watch your directories for changes and rebuild the site immediately, *and* it will make these changes available at http://localhost:1313/ so you can view your change in your browser. Go on, try it. This is one of the best ways to preview your site while working on it.

Committing Your Changes
-----------------------
When you're happy with the changes you can run these commands (line by line) in the command line

```
hugo 
git add .
git commit -m "message"
git push origin master
cd public
git add .
git commit -m "message"
git push gh-pages HEAD:gh-pages
```

What this is doing is:

* building the site using `hugo`
* staged those changes `git add .`
* committing those changes to the current branch `git commit -m "message"`, change message to something sensible
* pushing that commit to the server `git push origin master`
* changing to the public directory (where the site it built to) `cd public`
* staged those changes `git add .`
* committing those changes to the current branch `git commit -m "message"`, change message to something sensible
* pushing that commit to the branch to the gh-pages branch, which is the branch github uses for the website `git push gh-pages HEAD:gh-pages`

Learning More
-------------
To further learn Hugo and learn more, read through the Hugo [documentation](http://gohugo.io/overview/introduction).
