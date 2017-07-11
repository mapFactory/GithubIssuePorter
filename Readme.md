## Still in Development

## Github Issue porter
Suppose a repository on Github is no loner being maintained and no one has been given push access. 

The three methods that I know, 
1) ```git clone ...;  cd ...; git remote rm origin; git remote add ...; git push;```
2) ```git clone --bare ...; cd ...; git push --mirror ...;```
3) ```git clone --mirror ...; cd ...; git push --mirror ...;```
<br>https://stackoverflow.com/questions/3959924/whats-the-difference-between-git-clone-mirror-and-git-clone-bare

Two problems with all of these methods...
1) Issues are not ported over.
2) Pull requests are not ported over.

## Repo will currently aim to port issues not pull requests.
Program will get all issues via Github api.
for each issue will post to new repository.
https://developer.github.com/v3/issues/

## Potential Solution for Pull Requests
Clone the repository down. (they are by default read only)
<br>convert them over to local branches... with branch name of the original.
<br>push with all local branches.
<br>https://community.atlassian.com/t5/Bitbucket-questions/Cloning-a-pull-request/qaq-p/56394

## Please open Issue
If you know a better way to mirror that gets information simular to ownership transfer.
