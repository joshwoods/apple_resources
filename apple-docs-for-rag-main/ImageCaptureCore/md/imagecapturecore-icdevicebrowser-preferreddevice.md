

- ImageCaptureCore
- ICDeviceBrowser
-  preferredDevice 

Instance Property

# preferredDevice

Returns a device object that the client application should select when it launches.

macOS 10.4+

``` source
var preferredDevice: ICDevice? { get }
```

## Discussion

If the client application that calls this method is the autolaunch application associated with a device, and that device is the last one attached (through USB, FireWire, or network), then that device is the preferred device.

Call this method in the implementation of deviceBrowser(_:didAdd:moreComing:) if the value of `moreComing` is `false`; or in the implementation of deviceBrowserDidEnumerateLocalDevices(_:).

