

- AccessorySetupKit
-  ASMigrationDisplayItem 

Class

# ASMigrationDisplayItem

A previously-discovered accessory as presented by the discovery picker, for use when migrating it to AccessorySetupKit.

iOS 18.0+iPadOS 18.0+

``` source
class ASMigrationDisplayItem
```

## Mentioned in 

Discovering and configuring accessories

## Overview

Create instances of `ASMigrationDisplayItem` by calling the superclass’s initializer init(name:productImage:descriptor:), then specify the Bluetooth peripheralIdentifier, the Wi-Fi hotspotSSID, or both, for the specific accessory you want to migrate.

## Topics

### Accessory identifiers

var peripheralIdentifier: UUID?

The Bluetooth identifier of the accessory to migrate.

var hotspotSSID: String?

The Wi-Fi hotspot SSID of the accessory to migrate.

## Relationships

### Inherits From

- ASPickerDisplayItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Displaying picker items

class ASPickerDisplayItem

An accessory as presented by the discovery picker.

