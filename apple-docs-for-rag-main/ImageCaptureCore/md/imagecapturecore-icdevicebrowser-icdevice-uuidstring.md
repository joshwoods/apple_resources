

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  uuidString 

Instance Property

# uuidString

A string representation of the device’s universally unique identifier (UUID).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var uuidString: String? { get }
```

## See Also

### Identifying a Device

var name: String?

The device’s name as reported by the device module, or if no device module is in control of this device, by the device transport.

var productKind: String?

The device’s type.

var icon: CGImage?

The device’s icon image.

var persistentIDString: String?

A string representation of the device’s persistent ID.

var serialNumberString: String?

The device’s serial number.

