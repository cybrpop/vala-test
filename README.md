# testing

some testing with vala. making elementary apps to be specific lol. 
# Install it from source

You can of course download and install this app from source.

## Dependencies

Ensure you have these dependencies installed

* granite
* gtk+-3.0
* switchboard-2.0

## Install, build and run

```bash
# install elementary-sdk, meson and ninja
sudo apt install elementary-sdk meson ninja
# clone repository
git clone {{repository_url}} testing
# cd to dir
cd testing
# run meson
meson build --prefix=/usr
# cd to build, build and test
cd build
sudo ninja install && testing
```

## Generating pot file

```bash
# after setting up meson build
cd build

# generates pot file
ninja testing-pot

# to regenerate and propagate changes to every po file
ninja testing-update-po
```
