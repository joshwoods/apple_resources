

- Network Extension
-  Hotspot helper 

API Collection

# Hotspot helper

Integrate your app with the iOS hotspot network subsystem.

## Overview

NEHotspotHelper allows your app to participate in the process of authenticating with hotspot networks, that is, Wi-Fi networks where the user must interact with the network to gain access to the wider Internet. Hotspot helpers are only supported on iOS.

Important

NEHotspotHelper is *only* useful for hotspot integration. There are both technical and business restrictions that prevent it from being used for other tasks, such as accessory integration or Wi-Fi based location. Before using NEHotspotHelper, you must first be granted a special entitlement (`com.apple.developer.networking.HotspotHelper`) by Apple. For more information, see Hotspot Helper Request.

For more about creating a hotspot helper, see the Hotspot Network Subsystem Programming Guide.

## Topics

### Registration

class NEHotspotHelper

A class to register a hotspot helper.

### Commands

class NEHotspotHelperCommand

A command for the hotspot helper to handle.

class NEHotspotHelperResponse

The hotspot helper’s response to a command.

class NEHotspotNetwork

Information about a Wi-Fi network associated with a command or a response.

### Hotspot communication

Hotspot helpers can use these APIs to communicate with the hotspot even when Wi-Fi is not the default route.

func bind(to: NEHotspotHelperCommand)

Binds a URL request to the network interface associated with the hotspot helper command instance.

In-Provider Networking

Network APIs for use by all types of NetworkExtension providers and by hotspot helpers.

## See Also

### Wi-Fi management

Wi-Fi configuration

Add persistent Wi-Fi configurations, or temporarily move the device to a specific Wi-Fi network.

Configuring a Wi-Fi accessory to join a network

Associate an iOS device with an accessory’s network to deliver network configuration information.

