android-manifest
================

Welcome to the android-manifest wiki!
Getting Started
---------------
1.Get repo python/shell script file.

$mkdir -p ~/bin

$curl https://raw.github.com/xhteam/git-repo/default/repo > ~/bin/repo

$chmod +x ~/bin/repo

2.Put the ~/bin directory in your path of execution
  Make sure that the ~/bin directory you just created is in your path of execution 
so that you can easily run the repo command even when you're not in ~/bin. 
Assuming you are using the BASH shell, the default in recent versions of Ubuntu, 
you can set it like this:

$ export PATH=${PATH}:~/bin

  Or add it to your ~/.bashrc file.

3.To get started with xhteam github android manifest, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

4.Initialize your local repository using the CyanogenMod trees, use a command like this:

    repo init -u git://github.com/xhteam/android-manifest.git -b github

Then to sync up (This will cost long time per your internet speed,take a coffee:) now):

    repo sync

5.Prepare the device-specific code
  $source build/envsetup.sh
  $lunch xx per your developing board

How to build?
----------------------
  Generally it's same as standard android building. but we also prefer to provide some extra building 
commands to easily build different part.

$make bootimage      -->build standard kernel+ramdisk image

$make bootloader     -->build bootloader

$make otapackage     -->build recovery acceptable ota package

$mka bacon           -->build recovery acceptable ota package with MD5 checksum

$make updatepackage  -->build fastboot update supported package

Buildbot
--------

All supported devices are built nightly and periodically as changes are committed to ensure the source trees remain buildable.

TODO
