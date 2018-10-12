# simpleaur
A script for install packages from AUR that doesn't require extra dependences, only requires git installed. cower is only needed if you want to run simplesearch for find package names/updates in AUR (recommended). simpleaur does NOT have automatic dependency resolution.

# Instalation
`git clone https://gitlab.com/edu4rdshl/simpleaur.git`

ArchLinux users can install it from the PKGBUILD that is in AUR, type it commands:

```
$ mkdir simpleaur
$ cd simpleaur
$ curl -o PKGBUILD https://aur.archlinux.org/cgit/aur.git/plain/PKGBUILD?h=simpleaur-git
$ makepkg -sci
$ cd ..
$ rm -rf simpleaur/
```
# Usage
<b>For instalations: </b>
<code>./simpleaur package1 package2 package3 ...</code></br>

<b>For search: </b>
<code>./simplesearch text-to-search</code></br>

<b>For updated check: </b>
<code>./simplecheck</code>

You are free to move the scripts to /usr/bin and then use it's from everywhere. If you are using ArchLinux, install the <b>simpleaur-git</b> package from the AUR.
