

- AVFoundation
- AVCaptureDevice
-  isInUseByAnotherApplication 

Instance Property

# isInUseByAnotherApplication

A Boolean value that indicates whether another app is using the device.

Mac Catalyst 14.0+macOS 10.7+

``` source
var isInUseByAnotherApplication: Bool { get }
```

## Discussion

This property is key-value observable.

## See Also

### Accessing Device State

var isConnected: Bool

A Boolean value that indicates whether a device is currently connected to the system and available for use.

var isSuspended: Bool

A Boolean value that indicates whether the device is in a suspended state.

