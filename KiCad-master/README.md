KiCad
=====

KiCad modules, libraries, templates, and 3D models as created by AB2 Technologies.

[http://www.ab2tech.com](http://www.ab2tech.com "AB2 Technologies")

- - -

<div align="center"><a href="http://www.ab2tech.com"><img src="https://raw.github.com/ab2tech/KiCad/master/AB2Tech_300.png" alt="AB2 Technologies" /></img></div>

Description
-----------
We started using KiCad because we wanted to embrace a fully open-sourced and free solution. It's a powerful tool that is fully capable as a PCB design suite.

However, switching to KiCad meant sacrificing significant former efforts we put into creating vast libraries for our previous PCB design tool -- Eagle CAD. This frustrated us at first and significantly slowed our momentum as we transitioned to KiCad. We viewed losing all of our previous work as the single largest barrier to entry for KiCad. Although we really wanted to embrace the software for so many reasons, it was rather difficult to leave all of our existing content behind. As we struggled to get motivated, we began to realize that starting over in KiCad could be a good thing for us. We've learned a lot about consistency and best practices over time, but some of our initial work in Eagle didn't live up to some of our more developed standards. This meant with KiCad we'd get all that right from the beginning.

It also provided what we see as a tremendous opportunity to contribute to the KiCad community. By posting all of our libraries, modules, templates, and 3D models as we grow in KiCad, we're hoping everyone in the KiCad community can benefit as well. We have made tremendous strides with this content and it is fairly comprehensive for general purpose design activities.

Getting Started
---------------
The best way to get started with our content is to use it as the primary content repository for KiCad. This is rather simple thanks to some scripts we have included for installation.

Depending on target platform, use either the kicad_install.bat (Windows) or kicad_install.sh (Linux) script to create a symbolic link from the KiCad share directory to the AB2 KiCad directory. Alternatively, create the links manually. The Linux script will also prompt to sync all existing content into the AB2 KiCad directory.

If using Windows with newer versions of KiCad, manually configure the following environment variables to use our content (we'll add this to the script eventually):

    KISYSMOD="${KICAD_INSTALL_PATH}/modules"
    KISYS3DMOD="${KICAD_INSTALL_PATH}/3d_models"

Once the content is in place via symlink, simply use KiCad as normal. AB2Tech content is now available for use.

If using Arch Linux, an [AUR package](https://aur.archlinux.org/packages/kicad-library-ab2-git/) is available.  The libraries will need to be manually added to the library table.

Notes
-----
* Now that KiCad is stable with the v4.0+ releases, we have stopped supporting our legacy modules and are now deprecating them. It simply isn't practical for us to try and maintain them at this point. Keeping them in the repository seems to be an empty promise, so as of [`c49cad0`](https://github.com/ab2tech/KiCad/commit/c49cad0aa551aaa073e81186e0085f801f765bc1), the legacy modules will no longer be available on the master branch. We've created a tag called [`kicad-legacy-mods`](https://github.com/ab2tech/KiCad/releases/tag/kicad-legacy-mods) for anyone who wants to roll back, but you'll lose the benefits of all of our newer stuff. This seemed like the easiest way, sorry if we've hurt any feelings (and let us know with a Github "issue" if you need some help or disagree with our choice).
* Newer KiCad versions don't seem to render VRML2 very well. We've discovered that exporting these models to X3D using blender produces much better results. To that end, we've directed all ".pretty" modules to use X3D 3D models by default and legacy modules will use VRML2 models (X3D is not supported in legacy KiCad versions).
* Almost everything included here has the prefix AB2 in some form or fashion. This is not because we love ourselves so much, but rather to avoid any potential naming collisions (KiCad doesn't keep track of collisions)
* No guarantees, promises, or warranties are made regarding the content herein. We do our best to be accurate, but we encourage everyone to extensively validate on his or her own. Furthermore, we do not accept any liability, express or implied, related to the use or misuse of the content herein. Please enjoy our content responsibly!
* The KiCad content posted in this repository is done so under the Creative Commons license [CC BY-NC-SA 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)
* Please feel free to provide any and all feedback you have about our content. We always strive to improve what we're working on!

- - -

<div align="center"><a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/deed.en_US"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/3.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/deed.en_US">Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License</a></div>
