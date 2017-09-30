# README

## Summary

FiftyTwoFriends is a website for helping homeless folk and their friends manage couch-surfing arrangements during periods of homelessness and housing instability. Our belief is that many people are closer to homelessness than they think. By considering your social connections before it is necessary you can weave together a safety net for yourself using our platform. If you have 52 friends who would be willing to put you up for a week each year you will not have to sleep rough. Sleeping rough while homeless takes a major toll on one's health and wellness in many ways. We hope that FiftyTwoFriends will help people plan their periods of homelessness and allow them to recover housing more quickly as a result, while sharing the load amongst their full social network so as to not burn out any of their social connections. I, @roseaboveit, thought of this idea when I was homeless for six months. I worked hard to balance my social network, manage my couch surfing, while also doing an internship. FiftyTwoFriends is the application I wish I would have had for myself and my friends during that period.

This project uses rvm for ruby version management. This means we created a gemset that will store all the gems that you need for this project so that your other projects can avoid conflicts.


## Git workflow
In the following subsections, our process of working with Git is described. Feel free to submit a github issue if something is unclear.

### Fork from the "trunk" to your own Github profile
Log into your Github profile. Visit the [trunk](https://github.com/roseaboveit/FiftyTwoFriends), and click "Fork" (button at top-right of page).

### Clone to your local machine
The "52 Friends" source code is now forked to your Github profile.
To get the source code to your local machine, it varies by how your have your personal computer set up. Consult Github's documentation for how to set up, and work with, Git on your local machine. If you need help, let us know.

### Add an upstream remote
You now have a connection between your local machine and your github profile to start developing. The next step will be to add another remote so that you can get updates from the "trunk" and push your code up to be merged into our final product.
`git remote add upstream git@github.com:roseaboveit/FiftyTwoFriends.git`

### Create a new branch
To make it easier to work with multiple contributers use some identifying initials and info about the feature branch you are working on.
For example, this branch was created with the following command.
`git checkout -b wl_readme`

### Make changes to the source code, and push those to your Github fork and to the Upstream repository
These specifics vary by how your personal machine is set up--consult Github's documentation.
`git push origin branch_name`
^--- This command will allow you to interact with your branch on your own fork. This might be handy to leverage the tools of github when looking at your code. It also allows you to show off your code to others before it goes through the acceptance process on the main repository.
`git push upstream branch_name`
^--- This command will allow us to look at your feature in the upstream context. It is fine to wait on this one until you are pretty sure you are ready to submit a pull request. At this point people may start looking at your code to see what is coming down the pipeline.

### Make sure your code is ready for merge
A lot can change between the time that you have started working on a feature and the time that it is ready to submit for acceptance. We need to pull all those changes in and make sure that our feature is truly ready to go:
`git fetch upstream`
`git checkout master`
`git merge upstream/master`
`git checkout feature_branch`
`git rebase master`
If you can rebase cleanly then there won't be problems when you get to merging into the upstream project.
If there are any concerns fix them, commit them, and then repush your feature branch. Again, if you run into trouble, feel free to reach out for help.
`git push upstream feature_branch`


### Create pull request to trunk
At the [trunk](https://github.com/roseaboveit/FiftyTwoFriends), click on "New pull request" (top left corner).
Select the master branch as the branch the code is being pulled into.
Select the upstream version of your branch as the code being pulled. This should look like roseaboveit/feature_branch.
This leaves your origin branch free to work on adjustments as feedback comes in and to pull those adjustments into the upstream version of your branch through the github interface in case that is helpful visually.

### Communicate and Wait
This isn't a full time project. It can take some time to get your code looked at. Feel free to reach out by message on twitter (@roseaboveit) if you do not get a reasonably quick response. We will then look over the pull request and provide feedback. Once everything is cleared for merge we will merge the request.


##Authorship
README authored by: @roseaboveit and @boomzilla


## ToDos to consider including:

Things we may want to cover:

- [ ] Ruby version

- [ ] System dependencies

- [ ] Configuration

- [ ] Database creation

- [ ] Database initialization

- [ ] How to run the test suite

- [ ] Services (job queues, cache servers, search engines, etc.)

- [ ] Deployment instructions

- [ ] ...
