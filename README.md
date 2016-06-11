## TWRP device tree for Galaxy Note 4 (Europe, Oceanic, and Americas)

Add to `.repo/local_manifests/trlte.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/samsung/trlte" name="android_device_samsung_trlte" remote="TeamWin" revision="android-6.0" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_trlte-eng
make -j5 recoveryimage
```

Kernel sources are available at: https://github.com/jcadduono/nethunter_kernel_trlte/tree/twrp-5.1

