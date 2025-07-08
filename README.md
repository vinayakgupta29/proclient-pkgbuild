# proclient-pkgbuild

Instructions : 
- clone this repo using 
```git
git clone https://github.com/vinayakgupta29/proclient-pkgbuild.git
```
- and then download the PRO (Pokemon Revolution Online) CLient from 

<https://pokemonrevolution.net/download>

- put the downloaded tar.gz in the same folder as the PKGBUILD file

- Build the package using
```bash
makepkg -si --clean --cleanbuild
```
- Or for a cleaner build use the install.sh as
  ```bash
  chmod +x install.sh
  ./install.sh
  ```
