

- ImageCaptureCore
- ICDeviceBrowser
- 
  - ICDeviceBrowser
- ICDevice
- ICDeviceDelegate
-  deviceDidChangeSharingState(\_:) Deprecated

Instance Method

# deviceDidChangeSharingState(\_:)

Tells the delegate when the sharing state of a device changes.

macOS 10.4–10.15Deprecated

``` source
optional func deviceDidChangeSharingState(_ device: ICDevice)
```

## Discussion

Any Image Capture client application can choose to share the device over the network using the sharing or webSharing facility in Image Capture.

Execution of the delegate callback occurs on the main thread.

## See Also

### Responding to Device Changes

func deviceDidChangeName(ICDevice)

Tells the delegate when the name of a device changes.

