# Thorium-Special
Special builds of Thorium for SSE3, etc.

# *IMPORTANT!!*
# THIS REPO NOW ONLY HOSTS SSE3 BUILDS. For MacOS, Android, and Raspberry Pi, I have made new repositories for each one as per https://github.com/Alex313031/Thorium-Special/releases/tag/migrate-final Please find links in there.

<img src="https://github.com/Alex313031/Thorium-AVX2/blob/main/ThoriumLogo.png">

 -- <s>Simply a seperate repo for builds of Thorium https://github.com/Alex313031/Thorium that have modified compiler flags flags or args.gn flags for specific processors or use cases. I will sometimes put builds that don't need AVX here.

- NEW: Thorium Special now has builds for MacOS. Both x64 and ARM64 (for M1 Macs) are available. Kudos to @midzer for building them on his M1 Mac. &nbsp;<img src="https://raw.githubusercontent.com/Alex313031/Thorium/main/logos/STAGING/apple.png" width="29">
- NEW: Thorium Special now has ARM64 Raspberry Pi builds for the Pi 3B+ and Pi 4 The name will have ARM64 in the name. &nbsp;<img src="https://github.com/Alex313031/Thorium/blob/main/logos/STAGING/Raspberry_Pi_Logo.svg" width="28">
- NEW: Thorium Special now has Android Builds (ARM64 and ARM32) &nbsp;<img src="https://raw.githubusercontent.com/Alex313031/thorium/main/logos/STAGING/Android_Robot.svg" width="28">

&ndash; Windows builds are here > https://github.com/Alex313031/Thorium-Win \
&ndash; AVX2 builds are here > https://github.com/Alex313031/Thorium-AVX2/ &nbsp;<img src="https://github.com/Alex313031/Thorium/blob/main/logos/STAGING/AVX2.png" width="42">

Releases will have the architecture name in the name and the .deb package to differentiate them.

## Building <img src="https://github.com/Alex313031/Thorium/blob/main/logos/NEW/build_light.svg#gh-dark-mode-only"> <img src="https://github.com/Alex313031/Thorium/blob/main/logos/NEW/build_dark.svg#gh-light-mode-only">

Clone and do everything in https://github.com/Alex313031/Thorium except before building, copy the contents of one of the build.gn files in this repo to //chromium/build/config/compiler/, and modify as per below.

You can modify BUILD.gn (which goes in //chromium/build/config/compiler/) to suit your system by referring to the list of microarchitectures and associated -march flags here > https://gcc.gnu.org/onlinedocs/gcc/x86-Options.html
You can use the contents of ICELAKE.gn, BULLDOZER.gn, HASWELL.gn, MSSE4.2.gn, MSSE4.0.gn, or MSSE3.gn. Theoretically, any CPU supporting at least SSE3 can have their -march dialed in to specifically target them for best performance.

You could modify args.gn by referencing the args.list file (also in the regular Thorium repo).</s>

*Thanks for using Thorium!*

<img src="https://github.com/Alex313031/Thorium/blob/main/logos/STAGING/Thorium90_504.jpg" width="200">
