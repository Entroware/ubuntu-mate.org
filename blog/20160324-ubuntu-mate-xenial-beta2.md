<!--
.. title: Ubuntu MATE 16.04 Beta 2
.. slug: ubuntu-mate-xenial-beta2
.. date: 2016-03-24 20:00:00 UTC
.. tags: Ubuntu,MATE,Xenial,beta2,draft
.. link:
.. description: Ubuntu MATE 16.04 (Xenial Xerus) LTS Beta 2
.. type: text
.. author: Martin Wimpress
-->

We are preparing Ubuntu MATE Xenial Xerus (16.04) for distribution on
[April 21st, 2016](https://wiki.ubuntu.org/XenialXerus/ReleaseSchedule)
With this *Beta 1* pre-release, you can see what we are trying out in
preparation for our next (stable) version.

## What works?

People tell us that Ubuntu MATE is stable. You may, or may not, agree.

Ubuntu MATE *Beta Releases* are *NOT* recommended for:

  * Regular users who are not aware of pre-release issues
  * Anyone who needs a stable system
  * Anyone uncomfortable running a possibly frequently broken system
  * Anyone in a production environment with data or workflows that need to be reliable

Ubuntu MATE *Beta Releases* are recommended for:

  * Regular users who want to help us test by finding, reporting, and/or fixing bugs
  * Ubuntu MATE, MATE, and GTK+ developers

## What changed since the Ubuntu MATE 16.04 Beta 1 release?

First of all, I'd like to extend my thanks to:

  * **[Luke Horwell](https://ubuntu-mate.community/users/lah7/)** and [Robin Thompson](https://github.com/robint99)** for for their work on Ubuntu MATE Welcome and Software Boutique.
  * **[Gunnar Hjalmarsson](https://launchpad.net/~gunnarhj)** for his help making `im-config` and `gnome-language-selector` compatible with Ubuntu MATE.
  * **[Rico Tzschichholz](https://launchpad.net/~ricotz)** for his help completing MATE integration for Synapse.
  * **[Alexei Sorokin](https://build.opensuse.org/user/show/XRevan86)** and **[Alberts Muktupāvels](https://launchpad.net/~albertsmuktupavels)** for their help improving MATE integration in Compiz.
  * **[Timo Jyrinki](https://launchpad.net/~timo-jyrinki)** and **[Daniel Holbach](https://launchpad.net/~dholbach)** for sponsoring critical package updates for Ubuntu MATE.

<div align="center">
<img src="/gallery/blog/ubuntu-mate-1604-beta2.png" alt="Ubuntu MATE 16.04 Beta 2" />
</div>

Thanks to everyone else from the Ubuntu MATE community who contributed to this release!

### Here is what changed in Ubuntu MATE 16.04 Beta 2 since Beta 1.

  * Added Synapse 0.2.99.2-1
    * Synapse now features complete MATE integration. Synapse is
    installed by default but not active by default. It can be enabled
    via the updated MATE Tweak. 
  * Updated to MATE Tweak 3.5.7
    * Adds *Enable Launcher* to the *Interface* section which
    activates/deactives Synapse.
    * Fixes [LP: 1548011](https://bugs.launchpad.net/bugs/1548011)
  * Updated to Compiz
    * Improved MATE Compiz integration, `gtk-window-decorator` will now
    use settings from Marco when Compiz detects it is running in a MATE
    session.
    * Google Chrome and Chromium windows are considered Compiz windows
    in fullscreen to avoid tearing.
    * Refined the Compiz profile for MATE to correct some minor issues. 
  * Updated to Ubuntu MATE Welcome 16.04.3
  * Updated to Ubuntu MATE Artwork 16.04.3
    * Icon rendering in menus is faster.
    * Icon inheritance is fixed.
    * Corrected rendering of Mozo (menu editor) when using Ambiant-MATE
    and Radiant-MATE themes.
    * Fixes [LP: #1552363](https://bugs.launchpad.net/bugs/1552363),
    [LP: #1549079](https://bugs.launchpad.net/bugs/1549079),
    [LP: #1541929](https://bugs.launchpad.net/bugs/1541929),
    [LP: #1551029](https://bugs.launchpad.net/bugs/1551029),
    [LP: #1499521](https://bugs.launchpad.net/bugs/1499521),
    [LP: #1442738](https://bugs.launchpad.net/bugs/1442738),
    [LP: #1364073](https://bugs.launchpad.net/bugs/1364073)
  * Updated to Ubuntu MATE Settings 16.04.4
    * Auto-corrects pre-existing MATE incompatible input methods.
  * Fixed `im-config` and `gnome-language-selector`.
    *  Ensures a MATEvcompatible input method is selected by default.
    [LP: #1550325](https://bugs.launchpad.net/bugs/1550325)

<div class="bs-component">
    <div class="jumbotron">
        <h1>Download Ubuntu MATE 16.04</h1>
        <p>Join the fun and experience a retrospective future.</p>
        <a href="/xenial/" class="btn btn-primary btn-lg">Download</a>
        </p>
    </div>
</div>

## Known Issues

Here are the known issues.

### Ubuntu family issues

This is our known list of bugs that affect all flavours.

  * Cryptsetup password prompt is not shown.
    * [LP: #1359689](https://bugs.launchpad.net/bugs/1359689)
    * [LP: #1530548](https://bugs.launchpad.net/bugs/1530548)
  * Plymouth does not display the graphical boot splash.
    * [LP: #1370707](https://bugs.launchpad.net/bugs/1370707).
  * Shutdown/Restart of the live session does not work in Virtualbox and VMWare guests.
    * [LP: #1447038](https://bugs.launchpad.net/bugs/1447038)
  * The input box for editing a Wired connection static IP address doesn't appear correctly.
    * [LP: #1530323](https://bugs.launchpad.net/bugs/1530323)
  * Swap partition *may* fail to be created when installing on a disk with existing partitions.
    * [LP: #990744](https://bugs.launchpad.net/bugs/990744)

### Ubuntu MATE issues

This is our known list of bugs that jut affect Ubuntu MATE.

  * System Information in Ubuntu MATE Welcome displays "No Information Available".
  * Activating a Compton composited Window Manager in Virtualbox, without installing Guest Additions drivers, will lock up the desktop.
    * **VirtualBox drivers can be installed via Ubuntu MATE Welcome in the Getting Started section**.

The issues outlined above will be resolved via updates.

### PowerPC

  * Running Linux on PowerPC can require some tinkering and the following are useful references.
    * [PowerPC Known Issues](https://wiki.ubuntu.com/PowerPCKnownIssues)
    * [PowerPC FAQ](https://wiki.ubuntu.com/PowerPCFAQ)

You'll also want to check the Ubuntu MATE bug tracker to see what has already
been reported. These issues will be addressed in due course.

  * [Ubuntu MATE Bug Tracker](https://bugs.launchpad.net/ubuntu-mate)

## Feedback

Is there anything you can help with or want to be involved in? Maybe you just
want to discuss your experiences or ask the maintainers some questions. Please
[come and talk to us](https://ubuntu-mate.community/).