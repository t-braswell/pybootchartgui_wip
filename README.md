# pybootchartgui_wip
this is a quick rework of pybootchartgui, mainly done for the sake of antiX (sysVinit) and other linux distros not using systemd. with bootchartd folded into systemd, this package has fallen out of use.
Due to the package's age, there have been several deprecations:
1. dependencies include python (2.7); has beenupdated to python3. the same is true of the dependency python-cairo, this has been updated to python3-cairo. Trivial and finished.
2. python-gtk2 is deprecated, and there as been an attempt to move to Gobject-introspection
   (see https://packages.debian.org/buster/python-gtk2 and https://wiki.gnome.org/Projects/PyGObject/IntrospectionPorting)
   as a result, the gui.py script needs to be reworked Gobject, and the new dependencies need to be noted.

# TODO
1. rework gui.py for Gobjects
2. replace python-gtk2 dependency in /DEBIAN/contorl to reflect new dependencies
3. fix checksums
