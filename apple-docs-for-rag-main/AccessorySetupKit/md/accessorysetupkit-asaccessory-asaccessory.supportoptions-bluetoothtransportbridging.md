

- AccessorySetupKit
- ASAccessory
- ASAccessory.SupportOptions
-  bluetoothTransportBridging 

Type Property

# bluetoothTransportBridging

The accessory supports bridging to Bluetooth classic transport.

iOS 18.0+iPadOS 18.0+

``` source
static var bluetoothTransportBridging: ASAccessory.SupportOptions { get }
```

## Discussion

This option indicates that when connecting with low energy transport, the accessory supports activating Bluetooth classic transport profiles.

## See Also

### Bluetooth options

static var bluetoothPairingLE: ASAccessory.SupportOptions

The accessory supports Bluetooth Low Energy pairing.

static var bluetoothHID: ASAccessory.SupportOptions

The accessory supports Bluetooth Low Energy HID service.

