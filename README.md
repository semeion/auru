# auru
AUR Utility - Check foreign packages (typically installed w/ pacman -U) for available updates in AUR and author websites


This bash script will show you all packages with issues not reported by pacman and will track the website of developers to show you modifications on the projets.

That modifications happens before a package get updates on AUR. On this way you will know what packages will (or not) receive updates on AUR.

It is not an AUR helper, is more like a project tracker, used to obtain info about your installed packages directly from authors, not from AUR.

To see the modifications/news on console you need have `fzf` (optional dep) installed.


Manual installation
-------------------

Intall the deps and put `auru` on a folder and run with:
    `./auru --help`


Installing with git
-------------------

1) Clone the repository:
   `git clone https://github.com/semeion/auru.git`
   
2) cd into directory:
   `cd auru`
   
3) Install the deps with:
   `pacman -S python-html2text curl jq expac fzf`

4) Execute the script:
   `./auru --help`


Installation from AUR
---------------------

URL: https://aur.archlinux.org/packages/auru-git/

If you are using __Arch Linux__ (Manjaro, BlackArch, etc) do not need to install manually, copy the tarball from the AUR link above, extract on a temp dir, cd on it and type:

   `makepkg -i`

To uninstall run (as root):

   `pacman -R auru-git`





__<<< Contributors and Feedbacks are welcome! >>>__


Required deps
-------------
python-html2text, curl, jq, expac, fzf (optional)


Licensing
---------
auru is licensed under the GNU General Public License version 3 (GNU GPL v3).

_(C) 2019 Alexandre Bolelli_
