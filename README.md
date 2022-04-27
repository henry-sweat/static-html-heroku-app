# static-html-heroku-app

# create repo on github, then clone using SSH
$ git clone ...

# create files
$ echo " " > home.html 
$ echo '<?php include_once("home.html"); ?>' > index.php
$ echo '{}' > composer.json

# push files to github repo
$ git add .
$ git commit -m "initial commit"
$ git push origin main

# log in to heroku using CLI
$ heroku login

# set heroku as the remote
heroku git:remote -a your-app-name-123

# push repo to heroku
$ git add .
$ git commit -m "*"
$ git push heroku main

