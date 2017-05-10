
# Walkmod Parent

Parent project for walkmod and javacompiler for common customizing.

Simplifies application of global formattings.

You have to initilize the submodules after clone:

git clone ...
git submodule init
git submodule update

or you do a recursive clone

git clone --recursive ...

## Commands

The xml formmatter needs xmlstarlet and dos2unix:

```
sudo apt-get install xmlstarlet
sudo apt-get install dos2unix
```

`bin/format-xml`
> format xml files (see above for necessary tools!)


`bin/add-formatter-plugin`
> add formatter mavin plugin


`bin/format-java`
> execute formatter mavin plugin



`bin/mvn-clean-all`
> execute 'mvn clean' for all submodules


`bin/mvn-test-all`
> execute 'mvn test' for all submodules


`git submodule foreach git status -c | less`
> execute some command for each sub module (here: 'git status -c')



`bin/add-sub-modules`
> add non existing sub modules, add new or missing here and execute


## Infos

Uses git submodules: https://git-scm.com/book/en/v2/Git-Tools-Submodules

diff for all submodules:
> `git submodule foreach git diff -w | less`

status for all submodules:
> `git submodule foreach git status`

fetch and update all submodules:
> `git submodule update --remote`


Misc:
> `git diff --cached --submodule`

> `git diff --submodule`

