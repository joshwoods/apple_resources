

- DeviceDiscoveryExtension
- DDDevice
-  identifier 

Instance Property

# identifier

A unique identifier for the device.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
var identifier: String { get set }
```

## Discussion

As an example identifier for Bluetooth devices, your extension can use the device’s local name (see CBAdvertisementDataLocalNameKey).

## See Also

### Identifying the device

var displayName: String

A name for the device to display to the user.

var category: DDDevice.Category

An option that determies the icon that the picker UI displays for the device.

enum Category

An option that determines the icon for the device in the picker UI.

