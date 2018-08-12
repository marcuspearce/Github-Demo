========== GIT ==========
* Git vs GitHub
    * Git is a version/source control system 
    * GitHub is the application which utilizes Git tech
* Git Basics
    * git init - initialize
        * "ls -a" finds hidden folders (like ./git)
    * git status - asks for status
    * git add - add the files want git to keep track of (things to commit)
        * "git add ." adds all files to be in commit
    * git commit - making checkpoint in time w/ checkpoints added
        * "git commit -m ""  " - add comment w/ commit
* More Git
    * git log - shows record of all commits
        * PRESS "q" TO QUIT
    * git checkout - used for viewing smt else "checking out" like prev commit/branch
        * git checkout master - brings back to og
    * git revert --no-commit INSERT ID..HEAD - go back to given commit as if walking all subsequent commits back 
        * from stack overflow - das mah friend

========== HEROKU ==========
* heroku
    * heroku create - make url 
    * git remote -v - create url to push to 
    * git push heroku master - push in code from git (update code in project)
    * heroku logs - show error logs
        * To start need to add script to package.json "start: node app.js"
    * heroku run ___ - will run function in heroku server and return to this console
* Notes about Environmental Variables & Changing Databases
    * process.env._____ is environmental variable... smt that changes depending on server
    * fyi used "DATABASEURL"
        * in heroku.com used settings->configVars //DIDN'T WORK
        * heroku config:set MYCUSTOMVALUE=asdf //WORKED
    * to access mLab must use url found in website
        * for Yelpcamp: mongodb://marcus:asdf1234@ds163181.mlab.com:63181/yelpcamp 