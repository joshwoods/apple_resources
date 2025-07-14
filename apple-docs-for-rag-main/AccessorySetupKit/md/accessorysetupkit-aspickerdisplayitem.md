

- AccessorySetupKit
-  ASPickerDisplayItem 

Class

# ASPickerDisplayItem

An accessory as presented by the discovery picker.

iOS 18.0+iPadOS 18.0+

``` source
class ASPickerDisplayItem
```

## Mentioned in 

Discovering and configuring accessories

## Overview

Create instances of `ASPickerDisplayItem` that describe the accessories you want to discover. Each item contains a name and product image to display, plus an ASDiscoveryDescriptor that identifies the kind of accessories to match. Pass these in an array to showPicker(for:completionHandler:) to display a picker that allows the person using your app to discover and select nearby accessories.

Filter the matched accessories by supplying a descriptor, which contains various Bluetooth and Wi-Fi properties to match. The descriptor also allows you to set the bluetoothRange of matched accessories; set its value to ASDiscoveryDescriptor.Range.immediate to limit discovery of Bluetooth accessories to those within the immediate proximity of the device running your app.

To enable different behaviors during setup, use the setupOptions property, which is an option set (Swift) or bitfield (Objective-C) of behavior options. The defined options in ASPickerDisplayItem.SetupOptions allow you to specify behaviors like allowing renaming of the accessory during setup, or confirming accessory authorization before showing the setup view.

## Topics

### Creating a display item

init(name: String, productImage: UIImage, descriptor: ASDiscoveryDescriptor)

Creates a picker display item with a name and image to display and a descriptor to match discovered accessories.

### Specifying discovery properties

var descriptor: ASDiscoveryDescriptor

A descriptor that the picker uses to determine which discovered accessories to display.

### Customizing display properties

var name: String

The accessory name to display in the picker.

var productImage: UIImage

An image of the accessory to display in the picker.

### Customizing setup options

var setupOptions: ASPickerDisplayItem.SetupOptions

Custom setup options for the accessory.

struct SetupOptions

Setup options offered by the accessory picker.

var renameOptions: ASAccessory.RenameOptions

Options to allow renaming a matched accessory.

struct RenameOptions

Options that affect the behavior of an accessory renaming operation.

## Relationships

### Inherits From

- NSObject

### Inherited By

- ASMigrationDisplayItem

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

class ASMigrationDisplayItem

A previously-discovered accessory as presented by the discovery picker, for use when migrating it to AccessorySetupKit.

