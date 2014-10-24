colorschemer
============

There are a number of Vim plugins which convert a gui-only colorscheme to be useable with the terminal.
This plugin does the opposite. This is certainly a less common use case, but I if you happen to use
a 256 color only colorscheme (which I do), then this plugin will make gvim much more usable. In particular,
I was annoyed with the amount of manual effort to keep the gui attributes in sync with the constantly
evolving cterm attributes in my own yendor colorscheme.

Assuming you use vundle (which you should), you can install colorschemer by adding
```Plugin 'jlund3/colorschemer'``` to your .vimrc and running ```:PluginInstall```. Other package managers
will be similar. Once installed, if you run gvim and have a colorscheme loaded, then colorschemer will
automatically convert every cterm highlight attribute into the appropriate gui attribute.

Note that colorschemer requires that Vim be compiled with Python support. You can check this with
```:echo has('python')```.
