

- AccessorySetupKit
- ASAccessory
-  ssid 

Instance Property

# ssid

The accessory’s Wi-Fi SSID, if any.

iOS 18.0+iPadOS 18.0+

``` source
var ssid: String? { get }
```

## Mentioned in 

Discovering and configuring accessories

## Discussion

Use this identifier to establish a connection to the accessory.

## See Also

### Accessing identifiers

var bluetoothIdentifier: UUID?

The accessory’s unique Bluetooth identifier, if any.

var bluetoothTransportBridgingIdentifier: Data?

The accessory’s Bluetooth identifier, if any, for use when bridging classic transport profiles.

