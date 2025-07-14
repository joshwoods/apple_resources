

- Technotes
-  TN3135: Low-level networking on watchOS 

Article

# TN3135: Low-level networking on watchOS

Learn about the supported use cases for low-level networking on watchOS.

## Overview

watchOS groups networking into two categories:

- High-level networking. This includes the HTTP and HTTPS support in URLSession, and any code layered on top of that.

- Low-level networking. This includes Network framework, NSStream, and any other API that runs a TCP connection or UDP session directly. That includes the low-level aspects of URLSession, namely URLSessionStreamTask and URLSessionWebSocketTask. It also includes APIs, like NWBrowser and NSNetService, that interact directly with Bonjour.

watchOS allows all apps to use high-level networking equally. However, it only allows an app to use low-level networking under specific circumstances:

- It allows an audio streaming app to use low-level networking while actively streaming audio. Support for this was introduced in watchOS 6.

- It allows a VoIP app to use low-level networking while running a call using CallKit. Support for this was added in watchOS 9.

- It allows an app on watchOS to set up an application service listener so that the same app on tvOS can establish a low-level connection to it using the DeviceDiscoveryUI framework. Support for this was added in watchOS 9 and tvOS 16.

watchOS blocks low-level networking outside of these specific circumstances. For example, if a normal app attempts to start an NWConnection, that connection will stay in the .waiting(_:) state with an error of `ENETDOWN`. Similarly, an NWPathMonitor will remain in the .unsatisfied state.

Important

watchOS versions 6 through 8 had a bug where low-level networking might work outside of these circumstances (r. 83682211). That bug has been fixed in watchOS 9, which correctly enforces the rules described above.

The BSD sockets API doesn’t work for networking on watchOS under any circumstances. Use Network framework instead.

Foundation has various APIs for synchronously creating a value using bytes loaded from a URL. For example, init(contentsOf:) creates a data value in this way. Using these APIs with network URLs is not best practice on any Apple platform and is not supported by watchOS. Instead, load network URLs with a dedicated asynchronous networking API, like URLSession.

When writing watchOS networking code, test it on a real device; the simulator always allows low-level networking.

Also, test your networking code in a wide variety of network environments. Specifically, test it when the paired iPhone is available *and* when the paired iPhone is not available. The best way to test the latter is to turn off both Wi-Fi and Bluetooth in the Settings app on the iPhone. Do not use Control Center for this. For an explanation of the difference between these two mechanisms, see Use Bluetooth and Wi-Fi in Control Center.

For more information about building an audio streaming app for watchOS, see WWDC 2019 Session 716 Streaming Audio on watchOS 6.

## Revision History

- **2024-02-27** Fixed a typo.

- **2022-10-18** Added a discussion of the DeviceDiscoveryUI framework.

- **2022-09-27** Republished as TN3135. Updated with information about watchOS 9. Made significant editorial changes.

- **2021-05-14** Updated to call out that URLSessionStreamTask and URLSessionWebSocketTask are considered low-level networking.

- **2019-12-18** First published as “Low-Level Networking on watchOS” on Apple Developer Forums.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

