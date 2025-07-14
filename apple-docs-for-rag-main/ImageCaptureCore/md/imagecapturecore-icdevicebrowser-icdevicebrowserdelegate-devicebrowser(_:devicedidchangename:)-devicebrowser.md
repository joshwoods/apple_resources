

- ImageCaptureCore
- ICDeviceBrowser
- ICDeviceBrowserDelegate
-  deviceBrowser(\_:deviceDidChangeName:) 

Instance Method

# deviceBrowser(\_:deviceDidChangeName:)

Tells the delegate when the name of a device changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
optional func deviceBrowser(
    _ browser: ICDeviceBrowser,
    deviceDidChangeName device: ICDevice
)
```

## Discussion

A device’s name may change if a device module overrides the default name reported by the device’s transport layer, or if a user changes the name of the file system volume mounted by the device.

## See Also

### Responding to Device Changes

func deviceBrowser(ICDeviceBrowser, requestsSelect: ICDevice)

Tells the delegate when an event occurs on the device that may be of interest to the client application.

func deviceBrowser(ICDeviceBrowser, deviceDidChangeSharingState: ICDevice)

Tells the delegate when the sharing state of a device changes.

