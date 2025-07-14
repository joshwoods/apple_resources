

- Network Extension
-  NEHotspotConfigurationManager 

Class

# NEHotspotConfigurationManager

A manager that applies and removes hotspot configurations of Wi-Fi networks.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 7.0+

``` source
class NEHotspotConfigurationManager
```

## Overview

When your app creates a new hotspot configuration using NEHotspotConfiguration and applies it to a Wi-Fi network or attempts to update a previously configured network, the device prompts the user for approval. Without explicit user consent, your app can’t make configuration changes.

Your app can use removeConfiguration(forHS20DomainName:) or removeConfiguration(forSSID:) to delete a configuration that it has added, but not a configuration added by another app or user. The user can also delete configured networks using Settings \> Wi-Fi.

When your app is uninstalled, iOS removes the configurations of all networks your app has configured, including their keychain entries.

Hotspot Configuration Manager errors are listed in NEHotspotConfigurationError.

Important

To use the NEHotspotConfigurationManager class, you must enable the Hotspot Configuration capability in Xcode. For more information, see Hotspot Configuration Entitlement.

## Topics

### Creating configurations

class var shared: NEHotspotConfigurationManager

Instantiates NEHotspotConfigurationManager as a singleton, so it can be shared.

func apply(NEHotspotConfiguration, completionHandler: (((any Error)?) -> Void)?)

Adds or updates a Wi-Fi network configuration after prompting the user for permission, and then attempts to join the network under certain conditions.

### Getting a list of configurations

func getConfiguredSSIDs(completionHandler: ([String]) -> Void)

Submits a completion handler the configuration manager calls to send your app the names of the SSIDs or Wi-Fi hotspot domains in the configuration.

### Removing configuration

func removeConfiguration(forHS20DomainName: String)

Removes a Wi-Fi hotspot configuration, identified by a Hotspot 2.0 domain name, that your app previously added.

func removeConfiguration(forSSID: String)

Removes a Wi-Fi configuration, identified by an SSID, that your app previously added.

### Errors

let NEHotspotConfigurationErrorDomain: String

The domain string for errors involving hotspot configuration.

enum NEHotspotConfigurationError

Error values returned by hotspot configuration manager methods.

### Entitlements

Hotspot Configuration Entitlement

A Boolean value indicating whether your app can use the hotspot manager to configure Wi-Fi networks.

### Instance Methods

func joinAccessoryHotspot(ASAccessory, passphrase: String, completionHandler: (((any Error)?) -> Void)?)

func joinAccessoryHotspotWithoutSecurity(ASAccessory, completionHandler: (((any Error)?) -> Void)?)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Wi-Fi network configuration

class NEHotspotConfiguration

Configuration settings for a Wi-Fi network.

class NEHotspotEAPSettings

Extensible Authentication Protocol settings for configuring WPA and WPA2 enterprise Wi-Fi networks.

class NEHotspotHS20Settings

Settings for configuring Hotspot 2.0 Wi-Fi networks.

