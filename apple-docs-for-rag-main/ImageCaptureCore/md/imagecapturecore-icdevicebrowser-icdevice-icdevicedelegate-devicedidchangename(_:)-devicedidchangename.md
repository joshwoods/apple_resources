

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
- ICDeviceDelegate
-  deviceDidChangeName(\_:) 

Instance Method

# deviceDidChangeName(\_:)

Tells the delegate when the name of a device changes.

macOS 10.4+

``` source
optional func deviceDidChangeName(_ device: ICDevice)
```

## Discussion

This happens if the device module overrides the default name of the device reported by the device's transport layer, or if the name of the filesystem volume mounted by the device is changed by the user.

Execution of the delegate callback occurs on the main thread.

## See Also

### Responding to Device Changes

func deviceDidChangeSharingState(ICDevice)

Tells the delegate when the sharing state of a device changes.

Deprecated

