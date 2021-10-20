### Using git commands

**Create develop branch**

`git branch develop`: create `develop` branch

`git checkout develop`: switch to `develop` branch

`git push origin develop`: push `develop` branch from local to remote

**Create a feature branch**

`git branch feature/an-incredible-feature`

`git checkout feature/an-incredible-feature`

`git push origin feature/an-incredible-feature`

**Do some work**

Do some work in the `feature/an-incredible-feature` branch

**add, commit, push the new feature**

`git add`

`git commit -m "some comments"`

try `git push`: might not succeed since git is confused, set the upstream for this branch

**update develop with the new feature**

`git checkout develop`: go to the `develop` branch

`git merge feature/an-incredible-feature`: merge the new feature

*optional - delete the feature branch*

`git branch -D feature/an-incredible-feature`: delete the branch locally

`git push origin :feature/an-incredible-feature`: delete the branch remotely

### Using git flow

`git flow init`: connect keywords with the existing branches

`git flow feature start feature3`: create a new branch `feature/feature3` and switch to it

`git flow feature publish feature3`: switch to `feature/feature3` and push it to the `origin`

Do some work

`git flow feature finish feature3`: merge `feature/feature3` back to `develop` and delete it locally.

-   to remotely delete `feature/feature3` at the same time, use `git flow feature -F finish feature3`



