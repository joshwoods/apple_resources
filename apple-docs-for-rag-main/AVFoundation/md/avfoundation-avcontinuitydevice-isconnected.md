

- AVFoundation
- AVContinuityDevice
-  isConnected 

Instance Property

# isConnected

A Boolean value that indicates whether you can use the continuity device because it’s connected to the system.

tvOS 17.0+

``` source
var isConnected: Bool { get }
```

## Discussion

The value of the property can change from true to false, but not the reverse. Instead, the system creates a new AVContinuityDevice instance when the same physical device reconnects to the system.

