

- Xcode
- Capabilities
-  Configuring media device discovery 

Article

# Configuring media device discovery

Add a third-party media device or protocol as a streaming option in the same system menu as AirPlay.

## Overview

Enable the Media Device Discovery capability in an iOS app extension to indicate its intent to search the local network or paired Bluetooth devices for a third-party media receiver. This capability corresponds to the Media Device Discovery Extension entitlement. When you enable Media Device Discovery, Xcode adds the entitlement to a code-signing entitlements file for the extension’s target.

At run-time, when a user invokes a UI to play media, the app presents an AVRoutePickerView to offer possible devices for the user to stream to. The system searches your app’s bundle for extensions with this entitlement to check whether your app provides such a device. If so, the system adds the third-party device next to any available AirPlay devices in the picker, which provides the user with a unified media streaming experience.

## Add the Media Device Discovery capability to your target

To add the capability, follow the steps in the Add a capability section of Adding capabilities to your app for your extension’s target. If you add a new target in your Xcode project using the Media Device Discovery template, Xcode enables this capability automatically.

## Code the extension

You code the extension to search the local network or paired Bluetooth devices for a specific media receiver using the DeviceDiscoveryExtension framework. If the search succeeds, the extension passes the discovered device to the system. For an example app that demonstrates media device discovery, see Discovering a third-party media-streaming device.

## See Also

### Network

Configuring network extensions

Customize the various capabilities of your app’s networking stack, such as proxying DNS queries or creating packet tunnels.

Registering your app with APNs

Communicate with Apple Push Notification service (APNs) and receive a unique device token that identifies your app.

Configuring Group Activities

Leverage FaceTime infrastructure to create coordinated experiences users can share.

