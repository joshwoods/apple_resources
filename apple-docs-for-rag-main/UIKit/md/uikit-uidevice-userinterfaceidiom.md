

- UIKit
- UIDevice
-  userInterfaceIdiom 

Instance Property

# userInterfaceIdiom

The style of interface to use on the current device.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var userInterfaceIdiom: UIUserInterfaceIdiom { get }
```

## Discussion

For universal applications, you can use this property to tailor the behavior of your application for a specific type of device. For example, iPhone and iPad devices have different screen sizes, so you might want to create different views and controls based on the type of the current device.

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

var localizedModel: String

The model of the device as a localized string.

var identifierForVendor: UUID?

An alphanumeric string that uniquely identifies a device to the app’s vendor.

