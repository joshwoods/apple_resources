

- AccessorySetupKit
-  ASDiscoveryDescriptor 

Class

# ASDiscoveryDescriptor

Descriptive traits used to discover accessories.

iOS 18.0+iPadOS 18.0+

``` source
class ASDiscoveryDescriptor
```

## Mentioned in 

Discovering and configuring accessories

## Overview

Use an instance of this type to identify accessories your app can set up, then set it as the descriptor property of an ASPickerDisplayItem.

Some of the Bluetooth identifier properties work together to filter matching accessories, as described in the following table.

| Use | Filter property | Also requires | Description |
|----|----|----|----|
| Required | bluetoothServiceUUID or bluetoothCompanyIdentifier | (none) | Provide at least one UUID or manufacturer ID to filter. |
| Optional | bluetoothNameSubstring | bluetoothServiceUUID or bluetoothCompanyIdentifier | Provide a name substring to look for. Requires setting at least a service UUID or company ID, which identifies the service or company using the name. |
| Optional | bluetoothManufacturerDataBlob and bluetoothManufacturerDataMask | bluetoothCompanyIdentifier | When using manufacturer data filters, provide both the data and mask. These properties should have the same length and be less than or equal to the size of the advertised payload. The bluetoothCompanyIdentifier identifies the manufacturer associated with the data. |
| Optional | bluetoothServiceDataBlob and bluetoothServiceDataMask | bluetoothServiceUUID | When using UUID service data filters, provide both the data and mask. These properties should have the same length and be less than or equal to the size of the advertised payload. The bluetoothServiceUUID identifies the service associated with the data. |

The descriptor also allows you to set the bluetoothRange of matched accessories; set its value to ASDiscoveryDescriptor.Range.immediate to limit discovery of Bluetooth accessories to those within the immediate proximity of the device running your app.

## Topics

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

enum Range

The Bluetooth range in which to discover accessories.

### Specifying Wi-Fi properties

var ssid: String?

The SSID of the accessory’s Wi-Fi network.

var ssidPrefix: String?

The prefix string of SSID of the accessory’s Wi-Fi network.

### Specifying options

var supportedOptions: ASAccessory.SupportOptions

Options supported by an accessory.

struct SupportOptions

Options of discoverable accessories.

### Instance Properties

var bluetoothNameSubstringCompareOptions: NSString.CompareOptions

The accessory’s over-the-air Bluetooth name substring compare options.

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
- Sendable

## See Also

### Accessory discovery

class ASAccessoryEvent

Properties of an event encountered during accessory discovery.

enum ASAccessoryEventType

An enumeration of the types of events encountered during accessory discovery

