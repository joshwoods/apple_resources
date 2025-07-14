

- AccessorySetupKit
- ASAccessorySettings
-  bluetoothTransportBridgingIdentifier 

Instance Property

# bluetoothTransportBridgingIdentifier

A 6-byte identifier for bridging classic transport profiles.

iOS 18.0+iPadOS 18.0+

``` source
var bluetoothTransportBridgingIdentifier: Data? { get set }
```

## Discussion

AccessorySetupKit ignores this property if another app already authorized and bridged the accessory.

## See Also

### Inspecting accessory settings

var ssid: String?

A hotspot identifier that clients can use to connect to an accessory’s hotspot.

