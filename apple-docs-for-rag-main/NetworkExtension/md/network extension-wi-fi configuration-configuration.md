

- Network Extension
-  Wi-Fi configuration 

API Collection

# Wi-Fi configuration

Add persistent Wi-Fi configurations, or temporarily move the device to a specific Wi-Fi network.

## Overview

Using NEHotspotConfigurationManager, you can programmatically create two different types of Wi-Fi configurations:

- Persistent configurations, which are equivalent to the user joining a Wi-Fi network using the Settings app

- Join-once configurations, which temporarily move the device to a specific Wi-Fi network

The user must explicitly authorize both of these operations.

This API can help with a wide variety of tasks. For example, you can use it to help a user join a specific Wi-Fi network, like the hotspot at a local coffee shop, or to set up an accessory that uses Wi-Fi.

NEHotspotConfigurationManager supports a variety of authentication models:

- SSID with no authentication

- SSID with password-based authentication (WEP, WPA, and WPA2)

- SSID with EAP authentication

- Hotspot 2.0 with EAP authentication

NEHotspotConfigurationManager is only supported on iOS. For macOS, use the Core WLAN framework, which provides a full-featured Wi-Fi configuration and management API.

## Topics

### Essentials

Hotspot Configuration Entitlement

A Boolean value indicating whether your app can use the hotspot manager to configure Wi-Fi networks.

### Wi-Fi network configuration

class NEHotspotConfigurationManager

A manager that applies and removes hotspot configurations of Wi-Fi networks.

class NEHotspotConfiguration

Configuration settings for a Wi-Fi network.

class NEHotspotEAPSettings

Extensible Authentication Protocol settings for configuring WPA and WPA2 enterprise Wi-Fi networks.

class NEHotspotHS20Settings

Settings for configuring Hotspot 2.0 Wi-Fi networks.

## See Also

### Wi-Fi management

Configuring a Wi-Fi accessory to join a network

Associate an iOS device with an accessory’s network to deliver network configuration information.

Hotspot helper

Integrate your app with the iOS hotspot network subsystem.

