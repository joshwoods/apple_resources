

- AccessorySetupKit
- ASDiscoveryDescriptor
-  ASDiscoveryDescriptor.Range 

Enumeration

# ASDiscoveryDescriptor.Range

The Bluetooth range in which to discover accessories.

iOS 18.0+iPadOS 18.0+

``` source
enum Range
```

## Topics

### Creating an options instance

init?(rawValue: Int)

### Bluetooth options

case `default`

The default range in which to discover accessories.

case immediate

A range in the immediate vicinity of the device performing accessory discovery.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var bluetoothServiceUUID: CBUUID?

The accessory’s Bluetooth service UUID.

var bluetoothRange: ASDiscoveryDescriptor.Range

A property that tells the session to discover accessories within a specific Bluetooth range.

