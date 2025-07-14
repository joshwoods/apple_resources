

- ImageCaptureCore
- ICDeviceBrowser
-  stop() 

Instance Method

# stop()

Tells the delegate to stop looking for devices.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
func stop()
```

## Discussion

Calling this method frees all device instances that are not in use.

## See Also

### Browsing Devices

var isBrowsing: Bool

A Boolean value indicating whether the device browser is browsing for devices.

var devices: [ICDevice]?

All devices found by the browser.

class ICDevice

An abstract object that represents a device.

var browsedDeviceTypeMask: ICDeviceTypeMask

A mask whose set bits indicate the type of devices being browsed after the delegate receives the start message.

func start()

Tells the delegate to start looking for devices.

