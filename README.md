# android_device_asus_Z00A
Zenfone 2 ZE551ML Z00A

WIP CM Device tree for Asus Zenfone 2 ZE551ML Z00A

***MAJOR WIP***
May destroy phones, PC's and small kittens.... you've been warned!

To build this sucker:


mkdir cyanogen-12.1
cd cyanogen-12.1
repo init -u git://github.com/CyanogenMod/android.git -b cm-12.1
repo sync -j 20
. build/envsetup.sh
repopick -t zenfone2_bringup
repopick -t quick-charge-ui
breakfast Z00A
make -j (number of cores in your CPU +1)

And that should do it!
