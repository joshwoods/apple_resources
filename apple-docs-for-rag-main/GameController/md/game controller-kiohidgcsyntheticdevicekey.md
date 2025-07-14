

- Game Controller
-  kIOHIDGCSyntheticDeviceKey 

Global Variable

# kIOHIDGCSyntheticDeviceKey

A key that specifies whether the device is a game controller synthetic HID device.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kIOHIDGCSyntheticDeviceKey: String { get }
```

## Mentioned in 

Understanding game controller backward compatibility

## Discussion

This key is present with a Boolean value of `true` on all game controller synthetic HID devices that the Game Controller framework creates.

If your app needs to exclude these synthetic HID devices from discovery by IOHIDManagerRef, IOServiceGetMatchingServices(_:_:_:), or IOServiceAddMatchingNotification(_:_:_:_:_:_:), include the kIOHIDGCSyntheticDeviceKey with a value of `false` in the matching criteria.

```
```

Your code can check whether an io_service_t or an IOHIDDeviceRef refers to a game controller synthetic HID device by querying the value of the kIOHIDGCSyntheticDeviceKey property.

```
```

## See Also

### Game Controller framework migration from IOKit

Understanding game controller backward compatibility

Learn how macOS brings support for the latest game controllers to software that predates the introduction of the Game Controller framework.

