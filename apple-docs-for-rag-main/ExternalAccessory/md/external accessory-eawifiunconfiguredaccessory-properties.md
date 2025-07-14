

- External Accessory
- EAWiFiUnconfiguredAccessory
-  properties 

Instance Property

# properties

The properties the accessory supports.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var properties: EAWiFiUnconfiguredAccessoryProperties { get }
```

## See Also

### Getting Information About the Accessory

var name: String

The name of the accessory.

var manufacturer: String

The name of the accessory’s manufacturer.

var model: String

The model name of accessory.

var ssid: String

The Wi-Fi SSID of the accessory.

var macAddress: String

The primary MAC address of the accessory.

struct EAWiFiUnconfiguredAccessoryProperties

Options that can be combined using the C bitwise `OR` operator to represent the properties of an unconfigured accessory.

