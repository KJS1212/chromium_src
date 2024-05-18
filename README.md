# Building Chromium for Tegra 2 devices on Android credit to decatf because this is forked from there

I am basically just going to use the very bare minimum patches and arguements to get the browser to run so imma just remove a load of stuff because when I apply everything on the latest build, I get a ton of errors when compiling

what changed:

I simplified args.gn by basically removing pretty much everything but the neon stuff.

I deleted the ffmpeg stuff (this might break video but honestly, most of this stuff wasnt working anyway with the latest version of chromium from what I could tell. I mean, this is hundreds of lines of code and it was written years ago. Only the video fix patch seems to apply cleanly, but the two I left still both apply with errors

