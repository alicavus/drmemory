# Preface

Dr. Memory is a great tool for debugging memory related issues. Official releases are hosted freely on GitHub, but they lack of official .deb packages.

This repository is related to beginners, who prefer simple build and install without need of adding extra repositories or PPAs.

# How to build a .deb package?
Clone or download this repository:
```
git clone --depth=1 https://github.com/alicavus/drmemory.git
```

Then build (make) a package:
```
drmemory/build_deb
```

If you want a specific version, specify it:
```
drmemory/build_deb 2.6.20167
```

`drmemory-$VERSION.deb` should be generated in your current $PWD

# How to install that package?
Your graphical installer (like `gdebi`) should take care of it. `apt` or `dpkg` also will fullfil  same purpose.
```
sudo apt install "$(pwd)"/drmemory-*.deb
```


