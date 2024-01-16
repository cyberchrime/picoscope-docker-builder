Picoscope Podman Image
======================


Basics
======

To setup host system (need to run once):

    sudo ./picocmd setup


To run picoscope (pulling image if needed):

    ./picocmd run


To build locally (not necessary if you just want to run picoscope):

    ./picocmd build


By default, an Ubuntu-based image will be used.
For run & build commands, you can specify to use an OpenSUSE-based image instead:

    ./picocmd run opensuse

Or for Ubuntu:

    ./picocmd run ubuntu


The Ubuntu-based image is the default if no distro is specified.


Save data into your home directory, which is mounted to the same path in the
container as is on the host.

Data saved anywhere else will likely be lost when the container exits.


Details
-------

This requires the host to provide podman, bash v4+, udev, Wayland, which is by 
default installed on recent versions of Fedora.

It is tested only on: Kernel 6.6.8 / Fedora Linux 39 / / Docker 24
