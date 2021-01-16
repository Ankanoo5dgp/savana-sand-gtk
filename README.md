# gtk-theme-assembly-project

This repository contains the gtk- and graphical elements needed to assemble a GTK3-theme and gnome-shell with the purpose to create a-la-carte themes and providing the means to create a binary output

## How to make a theme?

## Notice: this repository contain elements which may not be finished! This is a 'working-environment' ! 

-create a file with the name of your theme,
-in this file you put the content of one of the 'barebone-files'
-within the gtk-3.0-file you drop the content of one of the 'theme-definers' you pick.
Finally choose a gnome-shell out of the repository Shells, copy the content.

So for example after choosing 'barebone-light', 'Standard-blue' and 'Wrk-PRO'-content
you file should have the following components:

-gnome-shell

-gtk-3.0

-copying


Withing the gtk-3.0 it should look like this:

-a folder 'global-graphics'

-a folder 'theme-colors' 

-a folder 'theme-graphics'

-G-gtk.css

-G-gtk-dark.css

-gtk.css

-gtk.gresource.xml

-main-dark.css

-main-light.css


Your file now has all the components needed to have a working theme.  This can be copied to your  '.themes'-folder on your computer.

If you want a optimized theme you can use the gtk.gresource.

## How to make a gresourced theme :

Go into the gtk3.0 file of your theme, open a terminal and execute the following command:
 glib-compile-resources gtk.gresource.xml
 
The result is: gtk.resource.

Make a new file (with the name of your final-theme) and copy the G-gtk.css, G-gtk-dark.css and the gtk.resource into that file.
Rename 'G-gtk.css' to 'gtk-css'
Rename 'G-gtk-dark.css' to gtk-dark.css

And that is it ! 

Your final theme-file should now only contain:

-gtk.css

-gtk-dark.css

-gtk.resource



