

- ImageCaptureCore
- ICDeviceBrowser
- ICDeviceBrowserDelegate
-  deviceBrowser(\_:deviceDidChangeSharingState:) 

Instance Method

# deviceBrowser(\_:deviceDidChangeSharingState:)

Tells the delegate when the sharing state of a device changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.13DeprecatedvisionOS 1.0+

``` source
optional func deviceBrowser(
    _ browser: ICDeviceBrowser,
    deviceDidChangeSharingState device: ICDevice
)
```

## See Also

### Responding to Device Changes

func deviceBrowser(ICDeviceBrowser, requestsSelect: ICDevice)

Tells the delegate when an event occurs on the device that may be of interest to the client application.

func deviceBrowser(ICDeviceBrowser, deviceDidChangeName: ICDevice)

Tells the delegate when the name of a device changes.

