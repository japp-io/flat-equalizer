# Troubleshooting

If you encounter issues while using the Flat Equalizer app, refer to the following troubleshooting tips to resolve common problems:

## Flat Equalizer Effects Not Working

Equalizer attaches itself to the media player that is currently playing. While most media players allow other apps to apply effects to their songs, some might require additional [configuration]. In some cases, certain media players do not allow external effects. In such situations, Equalizer will attach itself to the **Global Mix** as a fallback solution to support these players. Please note that this fallback may not be compatible with all devices.

## In-App Purchase No Longer Available

The in-app purchase is a one-time-only purchase without an expiry date. It's tied to your Google account. If your purchase is not detected by Wavelet, try clearing Play Store data by going to your system settings - apps. After rebooting your device, your purchase should be reloaded and made available to Wavelet again.

## Flat Equalizer Randomly Stopping

Certain OEMs implement aggressive battery-saving techniques, such as restricting applications from starting automatically or terminating apps even during active use. To avoid such issues, it's recommended to visit [dontkillmyapp.com] and follow the instructions specific to your device brand to prevent such problems from occurring.

## Legacy Mode Does Not Work via Bluetooth

If you're facing issues with Legacy Mode while using Bluetooth, navigate to your device's [developer options] and disable the "Disable Bluetooth A2DP hardware offload" setting.

## No Sound Difference via Bluetooth Device or External DAC

Some devices come with libraries that Wavelet uses, which might not support the sample rate of your Bluetooth device or external DAC. To address this problem for Bluetooth devices, access your device's [developer options] and set the Bluetooth sample rate to 48kHz and/or the Bluetooth codec to SBC. Unfortunately, there's no known solution for external DACs at this time.

## Clipping Issues on Samsung Devices

Certain Samsung devices feature a UHQ upscaler in the 'Sound quality and effects' system settings. To avoid clipping issues, switch the UHQ upscaler to "Bit upscaling only."

## Other

Flat Equalizer might not function as expected if other equalizer or hearing aid applications are installed. Examples include:
- Sound Assistant on certain Samsung devices
- AudioFX on LineageOS
- Third-party equalizer applications downloaded from the Play Store

If you encounter issues related to conflicting applications, freezing or uninstalling the problematic application and rebooting your device should resolve the issues.

[developer options]: https://developer.android.com/studio/debug/dev-options.html#enable
[dontkillmyapp.com]: https://dontkillmyapp.com/
[configuration]: supported-and-unsupported-music-players/#requires-additional-configuration
