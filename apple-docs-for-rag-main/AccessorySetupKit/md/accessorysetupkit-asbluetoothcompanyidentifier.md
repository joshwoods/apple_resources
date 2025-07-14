

- AccessorySetupKit
-  ASBluetoothCompanyIdentifier 

Structure

# ASBluetoothCompanyIdentifier

The identifier of a Bluetooth accessory provider.

iOS 18.0+iPadOS 18.0+Mac Catalyst

``` source
struct ASBluetoothCompanyIdentifier
```

## Topics

### Creating an identifier

init(UInt16)

init(rawValue: UInt16)

### Default Implementations

Equatable Implementations

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

enum Range

The Bluetooth range in which to discover accessories.

