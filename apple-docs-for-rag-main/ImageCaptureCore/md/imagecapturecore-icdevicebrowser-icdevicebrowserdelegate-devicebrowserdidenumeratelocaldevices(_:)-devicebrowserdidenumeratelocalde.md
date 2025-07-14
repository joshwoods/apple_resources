

- ImageCaptureCore
- ICDeviceBrowser
- ICDeviceBrowserDelegate
-  deviceBrowserDidEnumerateLocalDevices(\_:) 

Instance Method

# deviceBrowserDidEnumerateLocalDevices(\_:)

Tells the delegate that the device browser has completed sending deviceBrowser(_:didAdd:moreComing:) for all local devices.

macOS 10.4+

``` source
optional func deviceBrowserDidEnumerateLocalDevices(_ browser: ICDeviceBrowser)
```

## Discussion

Detecting locally connected devices (USB and FireWire devices) is faster than detecting devices connected using a network protocol. An Image Capture client application may use this message to update its user interface to let the user know that it has completed looking for locally connected devices and then started looking for network devices.

## See Also

### Adding and Removing Devices

func deviceBrowser(ICDeviceBrowser, didAdd: ICDevice, moreComing: Bool)

Tells the delegate that a device has been added.

**Required**

func deviceBrowser(ICDeviceBrowser, didRemove: ICDevice, moreGoing: Bool)

Tells the delegate that a device has been removed.

**Required**

