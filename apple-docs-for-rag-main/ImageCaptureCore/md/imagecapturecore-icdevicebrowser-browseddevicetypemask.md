

- ImageCaptureCore
- ICDeviceBrowser
-  browsedDeviceTypeMask 

Instance Property

# browsedDeviceTypeMask

A mask whose set bits indicate the type of devices being browsed after the delegate receives the start message.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 10.4+visionOS 1.0+

``` source
var browsedDeviceTypeMask: ICDeviceTypeMask { get set }
```

## Discussion

Construct this property by performing bitwise OR on values of ICDeviceTypeMask with values of ICDeviceLocationTypeMask. You can change this property while the browser is looking for devices.

## See Also

### Browsing Devices

var isBrowsing: Bool

A Boolean value indicating whether the device browser is browsing for devices.

var devices: [ICDevice]?

All devices found by the browser.

class ICDevice

An abstract object that represents a device.

func start()

Tells the delegate to start looking for devices.

func stop()

Tells the delegate to stop looking for devices.

