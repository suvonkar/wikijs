<!-- TITLE: Git -->
<!-- SUBTITLE: Wiki for Git -->

Home - http://localhost/

# Set Remote URL to avoid continuously asking for credentials: 
git remote set-url origin https://<username>:<password>@pswgithub.rds.lexmark.com/Indiaportal/LMS.git

https://stackoverflow.com/questions/34400272/visual-studio-code-always-asking-for-git-credentials/45517871#45517871

# Skipping password:
!   #   $    &   '   (   )   *   +   ,   /   :   ;   =   ?   @   [   ]
%21 %23 %24 %26 %27 %28 %29 %2A %2B %2C %2F %3A %3B %3D %3F %40 %5B %5D

https://stackoverflow.com/questions/6172719/escape-character-in-git-proxy-password

# Git migrate from one git to another:

`git clone --mirror https://suvonkar-es-kolkata@bitbucket.org/kolkataportal/lms.git`

*Make a bare mirrored clone of the repository*

`cd dashboard.git`
`git remote set-url --push origin https://pswgithub.rds.lexmark.com/Indiaportal/LMS.git`

*Set the push location to your mirror*

`git push –mirror`

https://stackoverflow.com/questions/22906917/how-to-move-git-repository-with-all-branches-from-bitbucket-to-github

# Install SSL certificate in Git:

Kofax Certificate URL : 
https://pswgithub.rds.lexmark.com/trupe/snips/blob/master/certificates/install_windows.md

Open Command promt.
Run "where git"
Open the folder upto '\Git'
Then go to 'mingw64\ssl\certs'
Edit ca-bundle.crt and paste the above url certificate code at the end and save

--------------------------------------------------------------------------------------
OR,
`git config --global http.sslVerify "false"`
or,
`git config --global http.sslVerify false`


# Creating an issue template for your repository

https://help.github.com/articles/creating-an-issue-template-for-your-repository/
