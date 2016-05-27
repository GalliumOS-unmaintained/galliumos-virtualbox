GalliumOS 2.x for VirtualBox & VMware
Release 20160527
https://coltondrg.com/galliumos-virtualbox/
https://galliumos.org/
Support IRC: #galliumos on freenode.net (ping ColtonDRG)

  GalliumOS for VirtualBox & VMware is a version of GalliumOS made for
developers who want to hack on GalliumOS without having to do devwork on a
Chrome device. Please note that this is NOT meant to represent the GalliumOS
experience, and it is not meant for end users. This is also not an official
GalliumOS build and should not be treated as such. GalliumOS for VirtualBox &
VMware is built on top of Ubuntu Server, and includes most of the software that
is included in a default GalliumOS install. It also includes the Firefox web
browser, the Atom text editor, VirtualBox or VMware drivers, an Nginx web
server daemon, and an OpenSSH daemon. The GalliumOS kernel is included, but
will not boot as it is known to cause issues with VirtualBox and VMware.
Instead, this uses the default Ubuntu kernel. GalliumOS for VirtualBox & VMware
has full access to all of the GalliumOS Xenon repos, including the prerelease
and testing repos. You may disable the prerelease and testing repos using the
normal galliumos-repodist method, but I recommend against it. I also recommend
that you go ahead and run GalliumOS Update to make sure that your system is up
to date.

The VirtualBox version is tested with VirtualBox 5.0.20+, and the VMware
version is tested with VMware Fusion 8 and VMware Workstation 12, though it
should work with any version of VMware compatible with the VMware 10
compatibility mode or later.

!!! WARNING !!!
  Don't add multiple CPU cores to this machine in VirtualBox. It causes a
problem with Xfce that I don't know how to fix. If you want to take a crack at
fixing it and let me know how you did it so I can fix it in a future release,
be my guest. I was unable to reproduce this issue on VMware, so if you must
have multiple CPU cores, use the VMware version.

!!! WARNING !!!
  Don't set this machine to compatibility level 12 in VMware. Compatibility
levels 10 and 11 work fine, but level 12 causes an issue. You shouldn't need
level 12 for any reason, as the only thing it enables over 11 is higher DirectX
support, which doesn't work in Linux anyway.

  One last thing. Be wary of the following packages
    - galliumos-laptop
    - galliumos-cbox
    - galliumos-sandy
    - galliumos-haswell
    - galliumos-broadwell
    - galliumos-baytrail
  These packages are not included in this install because they are hardware
support packages that only apply to Chrome hardware, and while they are
present on the typical GalliumOS install, they are known to break things in
VirtualBox and VMware.

  Thanks for checking out GalliumOS for VirtualBox & VMware, and thanks for
reading my readme. :)
