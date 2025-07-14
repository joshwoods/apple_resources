

- UIKit
- UIDevice
-  localizedModel 

Instance Property

# localizedModel

The model of the device as a localized string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var localizedModel: String { get }
```

## Discussion

The value of this property is a string that contains a localized version of the string returned from model.

## See Also

### Identifying the device and operating system

var name: String

The name of the device.

var systemName: String

The name of the operating system running on the device.

var systemVersion: String

The current version of the operating system.

var model: String

The model of the device.

var userInterfaceIdiom: UIUserInterfaceIdiom

The style of interface to use on the current device.

var identifierForVendor: UUID?

An alphanumeric string that uniquely identifies a device to the app’s vendor.

