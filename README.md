# MinMicroG_releases

Prebuilt flashable zips for the MinMicroG project - fork of the great work done by FriendlyNeighborhoodShane with further mods: 
- updates of permissions to allow smooth start on Android 14 (tested on Unihertz Jelly Max)
- fixes for debloating on systems where modern file-system is used: "/vendor", "/product" or "/system_ext" is where GApps are sitting, specifically GmsCore, GoogleServicesFramework, etc. otherwise there would be a race condition on boot.
- latest MicroG Services - com.google.android.gms - 0.3.3.240913
- latest MicroG Companion - com.android.vending - 0.3.3.40226

This package includes long list of items it debloats automatically and it might be tuned by adding/removing appropriate paths within `defconf` as `stuff_debloat` variable.

# This repo is only to hold release as I don't have time at the moment to port mods back whilst wanted to share with others like you to benefit from my mods on it.


The main README for the project:
 - https://github.com/bugsyb/MinMicroG/blob/master/README.md
 - Also inside the zips

Read the above document carefully before using any of the provided zip files.

Main repo for sources and build scripts:
 - https://github.com/bugsyb/MinMicroG

In the event of any damages to your device, house, ego barrier, baby,
relationships, galaxy, worldview, or in general the local fabric of
spacetime, I shall be held morally responsible, but in no way legally.

### How?
Built on my computer from MinMicroG's master using
```
  ./update.sh
  ./build.sh all
```

### Why a separate repo?
All modules have different version codes and I've never tagged in the
MinMicroG repo. (You could say that MinMicroG is rolling-release.)

### On what terms are they distributed?
Well, technically these zips are what the GPL considers 'aggregates',
collections of software. So all the individual components of the zip obey
their own licenses. The scripts that are part of MinMicroG are under GPLv3,
under my copyright. Most of the included software is also free software,
under license and copyright of their individual authors given in the zip's
readme. Exceptions are the various nonfree binaries packaged in some variant
zips.

### What's hidden inside contrib?
Oh, nothing. Just a bunch of lazy scripts I use myself to make MinMicroG releases,
along with a bunch of MinMicroG confs and hooks that may be interesting.
