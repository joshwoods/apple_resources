

- ImageCaptureCore
- ICDeviceBrowser
- ICDeviceBrowserDelegate
-  deviceBrowser(\_:requestsSelect:) 

Instance Method

# deviceBrowser(\_:requestsSelect:)

Tells the delegate when an event occurs on the device that may be of interest to the client application.

macOS 10.4+

``` source
optional func deviceBrowser(
    _ browser: ICDeviceBrowser,
    requestsSelect device: ICDevice
)
```

## Discussion

This message is sent when a button is pressed on a device and the current application is the target for that button press. When this happens, if a session is open on the device, this message is not sent to the browser delegate; instead the message `device(_:didReceiveButtonPress:)` is sent to the device delegate.

## See Also

### Responding to Device Changes

func deviceBrowser(ICDeviceBrowser, deviceDidChangeName: ICDevice)

Tells the delegate when the name of a device changes.

func deviceBrowser(ICDeviceBrowser, deviceDidChangeSharingState: ICDevice)

Tells the delegate when the sharing state of a device changes.

