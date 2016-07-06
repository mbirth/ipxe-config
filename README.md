iPXE Setup
==========

This is my [iPXE](http://ipxe.org/) setup. I use it to be able to boot
different antivirus and rescue products in my network. This is easier than
searching the little USB drive with the needed images on it.

I started out with @robinsmidsrod [config](https://gist.github.com/robinsmidsrod/2234639)
and went from there.


DNSMasq
=======

DNSMasq runs as a DHCP proxy for me. It'll enrich a DHCP response with the
needed data for remote booting. My config is in the `dnsmasq.d` folder and
needs to be copied to `/etc/dnsmasq.d/`.

The iPXE binary needs to be copied to `/var/ftpd/` and named `undionly.kpxe.0`.
(The `.0` missing from the filename in the DNSMasq config is intentional!)


Configured Images
=================

* [System Rescue CD](https://www.system-rescue-cd.org/)
* [DFSee](http://www.dfsee.com/)
* [CloneZilla](http://clonezilla.org/)
* [GParted Live](http://gparted.org/livecd.php)
* [g4u - ghost for unix](http://www.feyrer.de/g4u/)
* [G4L - Ghost for Linux](https://sourceforge.net/projects/g4l/)
* [AVG Rescue CD](http://www.avg.com/ww-en/avg-rescue-cd)
* [BitDefender Rescue CD](http://www.bitdefender.com/support/how-to-create-a-bitdefender-rescue-cd-627.html)
* [F-Secure Rescue CD](https://www.f-secure.com/en/web/labs_global/rescue-cd)
* [HDT - Hardware Detection Tool](http://www.hdt-project.org/)
* [Memtest86 V6](http://www.memtest86.com/)
* [Memtest86+ V5](http://www.memtest.org/)
