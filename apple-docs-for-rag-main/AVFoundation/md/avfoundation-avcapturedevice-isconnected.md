

- AVFoundation
- AVCaptureDevice
-  isConnected 

Instance Property

# isConnected

A Boolean value that indicates whether a device is currently connected to the system and available for use.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 2.1+

``` source
var isConnected: Bool { get }
```

## Discussion

When the value of this property is false for a particular capture device instance, it doesn’t become true again. If the same physical device reconnects, the system represents it as a new capture device instance.

You can key-value observe this property value to monitor when a device is no longer available.

## See Also

### Accessing Device State

var isSuspended: Bool

A Boolean value that indicates whether the device is in a suspended state.

var isInUseByAnotherApplication: Bool

A Boolean value that indicates whether another app is using the device.

