

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  name 

Instance Property

# name

The device’s name as reported by the device module, or if no device module is in control of this device, by the device transport.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var name: String? { get }
```

## Discussion

## See Also

### Identifying a Device

var productKind: String?

The device’s type.

var icon: CGImage?

The device’s icon image.

var uuidString: String?

A string representation of the device’s universally unique identifier (UUID).

var persistentIDString: String?

A string representation of the device’s persistent ID.

var serialNumberString: String?

The device’s serial number.

