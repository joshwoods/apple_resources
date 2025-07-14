

- AccessorySetupKit
- ASAccessory
-  bluetoothIdentifier 

Instance Property

# bluetoothIdentifier

The accessory’s unique Bluetooth identifier, if any.

iOS 18.0+iPadOS 18.0+

``` source
var bluetoothIdentifier: UUID? { get }
```

## Mentioned in 

Discovering and configuring accessories

## Discussion

Use this identifier to establish a connection to the accessory.

## See Also

### Accessing identifiers

var bluetoothTransportBridgingIdentifier: Data?

The accessory’s Bluetooth identifier, if any, for use when bridging classic transport profiles.

var ssid: String?

The accessory’s Wi-Fi SSID, if any.

