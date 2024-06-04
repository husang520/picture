

You should first make sure that your pc have git.exe and lfs.exe. You can check it with command /*git lfs install*/.

Then you can use git lfs to upload lager files.

The command is listed as:

git init #creat local repository enviroment

git lfs install # install lager files storage application

git lfs track *  # track the lager files that you want upload, * represent all of the files in this path.

git add .gitattributes # first add the attributes files(you must first use this command, or it will be failed.)

git commit -m "pre" # add the detail of the attributes files

git remote add origin https://***  

git push origin master # upload the attributes files

git add * # add the lager files of upload, * represent all of the files of the path

git commit -m "git LFS commit" # add the detail of lager files

git push origin master # upload lager files








