

- AdAttributionKit
-  Testing ad attributions with a downloaded profile 

Article

# Testing ad attributions with a downloaded profile

Reduce the time-window for ad attributions and inspect postbacks using a proxy during testing.

## Overview

Important

You can only use the AdAttributionKit testing profile for devices running OS versions earlier than iOS 18. In iOS 18 and later, the testing profile no longer works in AdAttributionKit or SKAdNetwork, so you need to use the AdAttributionKit Developer Mode. For more information see, Testing ad attributions with Developer Mode.

You can reduce the time-window for receiving ad attribution postbacks by installing an AdAttributionKit testing profile on your test device.

Download the latest profile by signing in to your Apple Developer account and then downloading the AdAttributionKit profile. This profile is compatible with both AdAttributionKit and SKAdNetwork.

For information about installing profiles, see Install a configuration profile on your iPhone or iPad. You can install this profile on devices running iOS or iPadOS 17.4 or later.

With this profile, the installed app has 5 minutes to update the conversion value after initially registering. The device sends the postback within another 5 minutes after the rolling 5-minute timer for conversion updates expires. Using this profile reduces the conversion value update and postback window from 24–48 hours to 5–10 minutes.

This testing profile expires 2 weeks after you install it on the device. To continue testing, download the latest profile and reinstall it.

Note

To test ad attributions, you need to log in to the device with a production Apple ID. AdAttributionKit doesn’t support sandbox Apple IDs.

## Inspect postbacks using an HTTP proxy

With this installed profile, the system can send AdAttributionKit postbacks through an HTTP proxy that you configure. By using an HTTP proxy, you can monitor the HTTP traffic between your device and the network, including AdAttributionKit postbacks. To configure the HTTP proxy, follow these steps on a testing device:

1.  Choose Settings \> Wi-Fi and select the Wi-Fi network you’re connected to.

2.  Under the HTTP Proxy heading, select Configure Proxy.

3.  Select Manual to configure the Server, Port, and Authentication settings for your proxy, or select Automatic to provide a URL for your proxy.

4.  Tap Save.

With the installed profile, the AdAttributionKit postbacks that the device sends go through the proxy.

## See Also

### Ad attribution testing

Testing ad attributions with Developer Mode

Reduce the time-window for ad attributions and inspect postbacks using a proxy during testing.

Creating postbacks in developer settings

Test development postbacks for your advertised app without interacting with ads from a publisher app.

