# AndroidLibXrayLite

## Build requirements
* JDK
* Android SDK
* Go
* gomobile

## Build instructions
1. `git clone [repo] && cd AndroidLibXrayLite`
2. `bash gen_assets.sh download && mkdir -p assets && cp -v data/*.dat assets/`
3. `python3 scripts/build_shared.py`

`libv2ray.aar` contains gomobile `libgojni.so` (VPN) and a `libxray.so` CLI launcher that loads the sibling library (ROOT), same layout as Asterisk4Magisk/AndroidLibXrayLite.
