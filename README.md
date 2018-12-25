# simpleaur
A script for install packages from AUR that doesn't require extra dependences, only requires git installed. cower is only needed if you want to run simplesearch for find package names/updates in AUR (recommended). simpleaur does NOT have automatic dependency resolution. It support PKGBUILDs download and other minor options (execute simpleaur -h).

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

```
Usage:
  simpleaur package1 package2        Install package1 and package2 from AUR.
  --help, -h                         Show it dialog.
  --purge, -p                        Delete all compiled packages in /home/sechacklabs/.simpleaur/Build.
  --download, -d                     Download all PKGBUILDS of packages passed as arguments in /home/sechacklabs/.simpleaur/pkgbuilds.
  --purgepkg, -pp                    Delete all downloaded PKGBUILDS in /home/sechacklabs/.simpleaur/pkgbuilds.
```

You are free to move the scripts to /usr/bin and then use it's from everywhere. If you are using ArchLinux, install the <b>simpleaur-git</b> package from the AUR.
