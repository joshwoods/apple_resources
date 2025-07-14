

- UIKit
- UIDevice
-  systemVersion 

Instance Property

# systemVersion

The current version of the operating system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var systemVersion: String { get }
```

## Discussion

An example of the system version is @“1.2”.

## See Also

### Identifying the device and operating system

var name: String

The name of the device.

var systemName: String

The name of the operating system running on the device.

var model: String

The model of the device.

var localizedModel: String

The model of the device as a localized string.

var userInterfaceIdiom: UIUserInterfaceIdiom

The style of interface to use on the current device.

var identifierForVendor: UUID?

An alphanumeric string that uniquely identifies a device to the app’s vendor.

