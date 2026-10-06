I'm not a programmer, I just needed this so I PROOOOOOMPted and figured I'd share it. Feel free to make changes or do whatever tf you want with it. Hopefully an actual programmer will take this and make something cooler out of it. 

gui/nxiso-gui.py is a single-file GTK4 front end (Python, PyGObject) that asks for an XISO file and an output folder, then runs nxiso -d <folder> -x <file> and shows the output. It runs natively on Wayland. It looks for nxiso in the NXISO environment variable, then next to the script, then in PATH.

Requirements: gtk4 and python-gobject.

I tested it on CachyOS with an Xbox 360 XISO and extraction worked. Feel free to change or drop it.
