

- External Accessory
- EAAccessory
-  firmwareRevision 

Instance Property

# firmwareRevision

The current firmware version for the accessory.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
var firmwareRevision: String { get }
```

## Discussion

The format of this string is determined by the accessory manufacturer.

## See Also

### Getting the Manufacturer-Supplied Attributes

var name: String

The display name of the accessory.

var manufacturer: String

The name of the accessory’s manufacturer.

var modelNumber: String

The model information for the accessory.

var serialNumber: String

The serial number of the accessory.

var hardwareRevision: String

The hardware version of the accessory.

var protocolStrings: [String]

The communication protocols supported by the accessory.

var dockType: StringDeprecated

