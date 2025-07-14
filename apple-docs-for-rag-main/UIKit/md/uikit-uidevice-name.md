

- UIKit
- UIDevice
-  name 

Instance Property

# name

The name of the device.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var name: String { get }
```

## Discussion

The default value of this property varies according to the device’s operating system version number:

| OS                 | Default value             | Example                  |
|--------------------|---------------------------|--------------------------|
| iOS 15 and earlier | User-assigned device name | `"Ravi’s iPhone 13 Pro"` |
| iOS 16 and later   | Generic device name       | `"iPhone"`               |

In iOS, the *user-assigned device name* is available in the Settings app under General \> About \> Name. To access the user-assigned device name through this property in iOS 16 and later, your app must meet certain criteria and be assigned an entitlement. For information, see com.apple.developer.device-information.user-assigned-device-name.

Related Sessions from WWDC22

Session 10096: What’s new in privacy

Session 10068: What’s new in UIKit

## See Also

### Identifying the device and operating system

var systemName: String

The name of the operating system running on the device.

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

