

- ImageCaptureCore
- ICDeviceBrowser
- ICDeviceBrowserDelegate
-  deviceBrowser(\_:didRemove:moreGoing:) 

Instance Method

# deviceBrowser(\_:didRemove:moreGoing:)

Tells the delegate that a device has been removed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
func deviceBrowser(
    _ browser: ICDeviceBrowser,
    didRemove device: ICDevice,
    moreGoing: Bool
)
```

**Required**

## Discussion

If several devices are removed at the same time, then this message is sent once for each device with the value of `moreGoing` set to `true` in each message except the last one.

## See Also

### Adding and Removing Devices

func deviceBrowser(ICDeviceBrowser, didAdd: ICDevice, moreComing: Bool)

Tells the delegate that a device has been added.

**Required**

func deviceBrowserDidEnumerateLocalDevices(ICDeviceBrowser)

Tells the delegate that the device browser has completed sending deviceBrowser(_:didAdd:moreComing:) for all local devices.

