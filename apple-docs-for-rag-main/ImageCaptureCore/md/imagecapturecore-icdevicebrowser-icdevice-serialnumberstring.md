

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  serialNumberString 

Instance Property

# serialNumberString

The device’s serial number.

macOS 10.4+

``` source
var serialNumberString: String? { get }
```

## Discussion

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

var persistentIDString: String?

A string representation of the device’s persistent ID.

