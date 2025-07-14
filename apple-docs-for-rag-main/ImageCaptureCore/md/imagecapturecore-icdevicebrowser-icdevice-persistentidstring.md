

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  persistentIDString 

Instance Property

# persistentIDString

A string representation of the device’s persistent ID.

macOS 10.4+

``` source
var persistentIDString: String? { get }
```

## See Also

### Identifying a Device

var name: String?

The device’s name as reported by the device module, or if no device module is in control of this device, by the device transport.

var productKind: String?

The device’s type.

var icon: CGImage?

The device’s icon image.

var uuidString: String?

A string representation of the device’s universally unique identifier (UUID).

var serialNumberString: String?

The device’s serial number.

