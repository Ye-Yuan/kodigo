#git

Initialize a submodule of an existing repo

    git submodule add <repo> <folder name>
    // ex.
    git submodule add https://github.com/keikun17/sigenasir_build.git build 

Change remote url

    // ex. Github Project 'islands' handed over to 'china' organization
    git remote set-url origin git@github.com:china

Update submodules

    git submodule foreach 'git fetch'

Reset state if you pulled the changes from the wrong remote branch (e.g. in develop branch then pulled a topic branch that's not ready yet)

    git reset --hard ORIG_HEAD 

Author + commit count

    git shortlog -s -n
