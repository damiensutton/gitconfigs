# gitconfigs
## How I sync my .gitconfig across may devices

I work with git on a lot of different systems. This is my method of synchronsing my git aliases, and most likely other git configurtion items, across the multiple environemnts I work with.

There are 2 steps
1. clone this repo the desired location on the system i am working on
2. add these line to my global .gitconfig
```
[include]
  path = <path/to/the/cloned/repo/.gitconfig-alias>
```
