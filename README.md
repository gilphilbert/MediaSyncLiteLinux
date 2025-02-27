## iBroadcast Media Sync Lite v0.4.2

A Linux-native graphical uploader for iBroadcast

## Build
### Requirements overview
- gcc
- make
- gtk+3.0 development files >= 3.10
- libcurl
- openssl
- libssl-dev
- libjansson (also available in ./jansson-2.7)

### Debian
The easist way to install for Debian is using the DEB package available in releases.

You can build the package manually as well:
```bash
sudo apt install build-essential libgtk-3-devlibcurl4-openssl-dev libjansson-dev
```
### Fedora
```bash
sudo dnf groupinstall "C Development Tools and Libraries"
sudo dnf install jansson-devel libcurl-devel gtk3-devel
```

## Compile
Just execute:
```bash
make
```

## Run
Now you can run MediaSync Lite from the directory where it was built:
```bash
./mediasynclite
```

## Install
You can optionall install MediaSync Lite so it's available system-wide:
```bash
sudo make install
```
The application will be installed in /usr/local/bin directory.

## Known issues
After uploading files, the app must be restarted to prevent those files from being uploaded again as duplicates.