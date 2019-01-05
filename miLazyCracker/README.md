# miLazyCracker
AUR-like automated build script for `nfc-tools/miLazyChacker` for `pacman` based distributions.

## Perculiarities
Note that this build is not entirely automated. One must obtain the source-code libraries `craptev1-v1.1.tar.xz` and `crapto1-v3.3.tar.xz`. These were originally available at [original site](http://crapto1.netgarage.org/), [archive.org mirror](https://web.archive.org/web/20180317133525/http://crapto1.netgarage.org).  
Since the license of these libraries restricts redistribution, it cannot be given freely. Instead, it is recommended that one ask the original producer at `blapost at gmail dot com`.  
Alternatively, since I obtained my copy from a more thorough search of the internet, you can probably get it this way too.

If none of these are suitable, it is possible to modify this build script, and the sources to use an alternative Crypto-1 bitsliced brute-forcer.

## How to install
makepkg --install
