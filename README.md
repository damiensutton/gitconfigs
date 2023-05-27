# gitconfigs

## How I sync my .gitconfig across all my devices

I work with git on a lot of different systems - Mac, Windows, Linux, personal, corporate or client specific hardware. When I don't have my git aliases available, I miss them. When I update my aliases, I want it to be easily replicated across all these systems. This is my method of synchronising my git aliases, and most likely other git configuration items, across the multiple environments I work with.

### Option 1: I have rights to install a cloud drive app e.g. Dropbox, OneDrive, Google Drive etc

1. Install the cloud drive and sign-in to sync my files.
2. Add the below [Include] section to my global .gitconfig, pointing to the .gitconfig-alias file in the cloud drive. Remember, the global .gitconfig should be in my home folder i.e cd ~

### Option 2: I only have git (not that that's a bad thing!)

1. Clone this repo the desired location on the system I am working on.
2. Add the below [Include] section to my global .gitconfig, pointing to the .gitconfig-alias file in the cloned repo.

#### The [Include] section on a Windows PC where I needed to clone this repo;

```
[include]
  path = "~///repos//gitconfigs//.gitconfig-alias"
```

#### and on my Windows "Parallels" version on my Mac where I have Dropbox installed;

```
[include]
  path = "\\\\Mac\\Dropbox\\GitConfigs\\.gitconfig-alias"
```


