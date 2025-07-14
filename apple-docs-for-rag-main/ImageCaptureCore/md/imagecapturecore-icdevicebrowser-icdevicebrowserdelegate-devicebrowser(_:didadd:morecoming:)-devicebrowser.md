

- ImageCaptureCore
- ICDeviceBrowser
- ICDeviceBrowserDelegate
-  deviceBrowser(\_:didAdd:moreComing:) 

Instance Method

# deviceBrowser(\_:didAdd:moreComing:)

Tells the delegate that a device has been added.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
func deviceBrowser(
    _ browser: ICDeviceBrowser,
    didAdd device: ICDevice,
    moreComing: Bool
)
```

**Required**

## Discussion

If several devices are found during the initial search, then this message is sent once for each device with the value of `moreComing` set to `true` in each message except the last one.

Not all devices are reported using this method. Devices that fail to communicate successfully are silently ignored.

## See Also

### Adding and Removing Devices

func deviceBrowser(ICDeviceBrowser, didRemove: ICDevice, moreGoing: Bool)

Tells the delegate that a device has been removed.

**Required**

func deviceBrowserDidEnumerateLocalDevices(ICDeviceBrowser)

Tells the delegate that the device browser has completed sending deviceBrowser(_:didAdd:moreComing:) for all local devices.

