

- UIKit
- UIDevice
-  systemName 

Instance Property

# systemName

The name of the operating system running on the device.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var systemName: String { get }
```

## See Also

### Identifying the device and operating system

var name: String

The name of the device.

var systemVersion: String

The current version of the operating system.

var model: String

The model of the device.

var localizedModel: String

The model of the device as a localized string.

var userInterfaceIdiom: UIUserInterfaceIdiom

The style of interface to use on the current device.

var identifierForVendor: UUID?

An alphanumeric string that uniquely identifies a device to the app’s vendor.

