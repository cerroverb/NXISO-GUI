I'm not a programmer, I just needed this so I PROOOOOOMPted and figured I'd share it. Feel free to make changes or do whatever tf you want with it. Hopefully an actual programmer will take this and make something cooler out of it. The clanker built it on Ubuntu, but I can confirm it works on Arch and Artix Wayland. Converted my entire set of remaining ISOs in my library with it.  

src/nxiso-gui.c: small GTK4 window. Pick an ISO (or drag it onto the window), pick an output folder (auto-filled next to the ISO), press Extract. Runs nxiso -x -d <folder> <iso> and shows the output, then a success or failure popup.
build-appimage.sh: builds nxiso with the existing Makefile, builds the GUI, and packs both into NXISO_Extract-x86_64.AppImage with linuxdeploy + the GTK plugin. Native Wayland (the plugin's forced GDK_BACKEND=x11 is removed).
nxiso-gui.desktop, nxiso-gui.svg, README.md, LICENSE.

Built on Ubuntu 24.04. Extraction tested under X11, and the window confirmed opening natively on Wayland.

Feel free to change it, drop it, or attach the AppImage to releases. 
