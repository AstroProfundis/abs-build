abs-build
=========

My custom build packages for ArchLinux, including all [my AUR](https://github.com/AstroProfundis/aur) [packages](https://aur.archlinux.org/packages/?SeB=m&K=AstroProfundis) and some custom modified ones from other's AUR. Some packages are build with `clang`.

> Note that `i686` arch is not maintained anymore and packages may be out-dated.

Binary repository can be used:

`/etc/pacman.conf`:

    [aspro]
    SigLevel = Optional TrustAll
    Server = http://repo.hoshi.at/archlinux/$arch

And you may need to sign my packaging key, otherwise you'll probably have issues installing packages:

    sudo pacman-key -r C75827D8 # get the key
    sudo pacman-key --lsign-key C75827D8

This key is available on any public keyservers and also available [here](http://repo.hoshi.at/archlinux/pubring.gpg).

Read more about `pacman-key` on [wiki](https://wiki.archlinux.org/index.php/Pacman-key).
