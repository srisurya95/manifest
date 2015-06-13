The Android Open Source Project+RRO Lollipop 5.1
===========

To initialize your local repository using the AOSP trees, use a command like this:
````bash
repo init -u git://github.com/srisurya95/manifest.git -b lollipop-5.1
```
Add Moto G resources by typing this:
````bash
curl --create-dirs -L -o .repo/local_manifests/moto-msm8226.xml -O -L https://raw.githubusercontent.com/srisurya95/manifest/aosp-5.1/moto-msm8226.xml
```
Then to sync up:
````bash
repo sync
```
Finally to build:
````bash
./build.sh device_codename
```
Example:
````bash
./build.sh falcon
```
