

- AccessorySetupKit
- ASDiscoveryDescriptor
-  bluetoothServiceUUID 

Instance Property

# bluetoothServiceUUID

The accessory’s Bluetooth service UUID.

iOS 18.0+iPadOS 18.0+

``` source
@NSCopying
var bluetoothServiceUUID: CBUUID? { get set }
```

## Mentioned in 

Discovering and configuring accessories

## See Also

### Specifying Bluetooth properties

var bluetoothCompanyIdentifier: ASBluetoothCompanyIdentifier

The accessory’s 16-bit Bluetooth Company Identifier.

struct ASBluetoothCompanyIdentifier

The identifier of a Bluetooth accessory provider.

var bluetoothManufacturerDataBlob: Data?

A byte buffer that matches the accessory’s Bluetooth manufacturer data.

var bluetoothManufacturerDataMask: Data?

The accessory’s Bluetooth manufacturer data mask.

var bluetoothServiceDataBlob: Data?

A byte buffer that matches the accessory’s Bluetooth service data.

var bluetoothServiceDataMask: Data?

The accessory’s Bluetooth service data mask.

var bluetoothNameSubstring: String?

The accessory’s over-the-air Bluetooth name substring.

var bluetoothRange: ASDiscoveryDescriptor.Range

A property that tells the session to discover accessories within a specific Bluetooth range.

enum Range

The Bluetooth range in which to discover accessories.

