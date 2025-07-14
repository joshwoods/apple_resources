

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
-  requestYield() Deprecated

Instance Method

# requestYield()

Requests that device module in control of this device yield control.

macOS 10.4–10.15Deprecated

``` source
func requestYield()
```

## Discussion

Use this method only if the client will communicate with the device directly. The device module may not yield control of the device if it has an open session.

## See Also

### Deprecated Symbols

func requestEjectOrDisconnect()

Requests to eject the media if permitted by the device, or to disconnect from a remote device.

Deprecated

var moduleExecutableArchitecture: Int32

The executable architecture of the device module servicing the requests.

Deprecated

