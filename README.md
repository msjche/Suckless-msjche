# .local-bin-scripts

You will need my scripts in your $PATH in order for the dwmblocks bar to populate.  Please refer to this repo:

	https://github.com/msjche/.local-bin-scripts

Once scripts are added and accessible:

Installation:

	git clone https://github.com/msjche/Suckless-msjche ~/Suckless
	cd ~/Suckless/dwm && sudo make clean install
	cd ~/Suckless/dwmblocks && sudo make clean install
	cd ~/Suckless/dmenu && sudo make clean install
	cd ~/Suckless/st && sudo make clean install

I have chosen to use the alacritty terminal for normal use.  However, st is used for the scratchpad functionality.  If on Arch-based distro:

	sudo pacman -S alacritty

You may also change to using st for all functions by editing the following line:

	vim ~/Suckless/dwm/config.h

edit:

	static const char *termcmd[]	= { "alacritty", NULL };

to read:

	static const char *termcmd[]	= { "st", NULL };

Then recompile (while in ~/Suckless/dwm

	sudo make install

Cheers!
