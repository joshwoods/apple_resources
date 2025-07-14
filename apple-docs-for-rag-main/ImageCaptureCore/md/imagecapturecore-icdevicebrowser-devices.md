

- ImageCaptureCore
- ICDeviceBrowser
-  devices 

Instance Property

# devices

All devices found by the browser.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var devices: [ICDevice]? { get }
```

## Discussion

This array is empty before the first invocation of the delegate method deviceBrowser(_:didAdd:moreComing:). The value of this property changes as devices appear and disappear.

## See Also

### Browsing Devices

var isBrowsing: Bool

A Boolean value indicating whether the device browser is browsing for devices.

class ICDevice

An abstract object that represents a device.

var browsedDeviceTypeMask: ICDeviceTypeMask

A mask whose set bits indicate the type of devices being browsed after the delegate receives the start message.

func start()

Tells the delegate to start looking for devices.

func stop()

Tells the delegate to stop looking for devices.

