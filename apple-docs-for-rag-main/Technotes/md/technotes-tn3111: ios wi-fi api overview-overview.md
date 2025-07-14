

- Technotes
-  TN3111: iOS Wi-Fi API overview 

Article

# TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

## Overview

iOS does not have a general-purpose API for Wi-Fi scanning and configuration. However, it does support a wide range of special-purpose Wi-Fi APIs. This technote lists some use cases supported by those special-purpose APIs.

## Navigate an internet hotspot

If your app helps the user navigate an internet hotspot — a Wi-Fi network where the user must interact with the network to gain access to the wider internet — adopt the Hotspot helper API.

To use `NEHotspotHelper` you must first be granted a special entitlement (`com.apple.developer.networking.HotspotHelper`) by Apple. For information on how to apply for this, see Hotspot helper.

Important

`NEHotspotHelper` is *only* useful for hotspot integration. There are both technical and business restrictions that prevent it from being used for other tasks, such as accessory integration or Wi-Fi based location.

## Add an accessory to the user’s network

If you’re creating a hardware accessory and you want to make it easy for the user to add it to their local network, your best option is to build your accessory with that in mind. Use one of these approaches:

- Wireless Accessory Configuration (WAC) — The user can configure a WAC-capable accessory directly in Settings. Optionally, use EAWiFiUnconfiguredAccessoryBrowser to integrate accessory configuration directly in your app.

- HomeKit — Call `HMHome` APIs like performAccessorySetup(using:completionHandler:) to ask the system to scan for, pair, and configure any unpaired HomeKit accessories .

Important

To add WAC or HomeKit support to your accessory, join the MFi Program.

If your accessory does not support WAC or HomeKit, you can build an accessory configuration experience on top of `NEHotspotConfigurationManager`, although this will not be as seamless as the WAC and HomeKit accessory experience. For an example of how you might approach this, see Configuring a Wi-Fi accessory to join a network.

## Temporarily join a network

If your app needs to temporarily join a Wi-Fi network — for example, you want to interact with a Wi-Fi enabled accessory with its own independent network — use `NEHotspotConfigurationManager` and set joinOnce to true. For more details, see Wi-Fi configuration.

If you’re working with a Wi-Fi accessory, use AccessorySetupKit to simplify discovery and configuration of your accessory.

## Permanently join a network

Some apps need to configure the iOS device to permanently join a Wi-Fi network, as if the user had selected the network in Settings \> Wi-Fi. For example, an app from an ISP might do this to get the user’s iOS device on to the Wi-Fi network published by a new DSL gateway that they’ve just installed. If your app needs to do this, use `NEHotspotConfigurationManager` and set joinOnce to false. For more details, see Wi-Fi configuration.

## Peer-to-peer networking

If your goal is to communicate with other nearby devices, look at:

- Network framework

- Multipeer Connectivity framework

Both of these support networking over peer-to-peer Wi-Fi. In Network framework you must opt in to this via the includePeerToPeer property. For more information about peer-to-peer networking, see TN3151: Choosing the right networking API.

Important

The on-the-wire protocol used by these peer-to-peer networking APIs is not documented for third-party use, so this technique only works between Apple devices.

## Location tracking

If you’d like to use Wi-Fi data to determine the device’s location, use Core Location. This locates the device using a wide variety of techniques, including Wi-Fi. For more information, see Maps and Location.

## Current Wi-Fi network

If you need to know the name of the device’s current Wi-Fi network, call fetchCurrent(completionHandler:). That method requires iOS 14 or later. On older systems, call CNCopyCurrentNetworkInfo.

## Revision History

- **2024-09-24** Added information about AccessorySetupKit. Added a link to TN3151. Made other minor editorial changes.

- **2022-05-24** Made minor editorial changes.

- **2022-02-08** Republished as TN3111. Broke the content into task-focused sections. Added a link to Configuring a Wi-Fi accessory to join a network. Added a reference to fetchCurrent(completionHandler:). Updated the text for the new publication platform.

- **2017-08-14** Added information about `NEHotspotConfigurationManager`.

- **2016-11-16** First published as QA1942 ”iOS Wi-Fi Management APIs”.

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

TN3158: Resolving Xcode 15 device connection issues

Identify software preventing Xcode 15 from connecting to Apple devices, and modify your configuration to allow these connections.

