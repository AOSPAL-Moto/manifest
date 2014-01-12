Unofficical Paranoid Android by [AOSPAL](http://google.com/+AospalOrg)
======================================================================

Paranoid SaberDroid
===================

SaberMod Linaro GCC Optimized PA
================================

[Official PA Source Is Here](https://github.com/AOSPA-legacy)
------------------------------------------------------

Building AOSPAL
-------------------------

To get started with AOSPAL, you'll need to get
familiar with [Git and Repo](http://source.android.com/download/using-repo).

To initialize your local repository using the ParanoidAndroid trees, use a command like this:

    repo init -u git://github.com/AOSPAL/manifest.git -b remix-legacy

Then sync up AOSPAL:

    repo sync
    
Then download additional repo's for unofficial devices:

    curl -L -o .repo/local_manifests/roomservice.xml -O -L https://raw.github.com/ASOPAL-Moto/manifest/remix-legacy/roomservice.xml
 
    	( or Download: https://github.com/AOSPAL-Moto/manifest/blob/remix-legacy/roomservice.xml
		and place it in your ~/Android/.repo/local_manifests/roomservice.xml (or ~/'name you choose'/.repo/local_manifests/ )

Then sync up:

    repo sync

For information on how to build, check [Here](https://github.com/AOSPA-Moto/manifest)

Building Our Custom Flavor of Paranoid Android
----------------------------------------------

Build:

    ./rom-build.sh <YOUR_DEVICE>
