## Welcome to LegendROM wiki

You can use the following guide to build LegendROM for your devices. Please check the list of devices supported currently.


### Setup

Follow the given code block to setup the initial repo

```
#1. Make directory where we can start building and cd into it
mkdir LegendROM && cd LegendROM

#2 Download the repo tool from google and give appropriate permissions to work
curl https://storage.googleapis.com/git-repo-downloads/repo-1 > /bin/repo && chmod +x repo/bin/

#3 Initialise the manifest for SymphonyOS
repo init -u https://github.com/LegendROM/manifest -b 11

#4 Download the source 
repo sync -j16

#6 Setup the build environment and start building for SymphonyClassroom
source build/envsetup.sh
lunch <device-name>-<build-type>
make otapackage
```


### Support or Contact

Having trouble with building? Cantact us on pranavthombare97@gmail.com
