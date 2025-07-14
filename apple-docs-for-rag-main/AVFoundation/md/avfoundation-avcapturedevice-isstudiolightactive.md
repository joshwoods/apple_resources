

- AVFoundation
- AVCaptureDevice
-  isStudioLightActive 

Instance Property

# isStudioLightActive

A Boolean value that indicates whether Studio Light is active on a device.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+

``` source
var isStudioLightActive: Bool { get }
```

## Discussion

When the value is true, the system artificially lights the subject’s face to simulate the presence of a studio light near the camera.

## See Also

### Configuring Studio Light

class var isStudioLightEnabled: Bool

A Boolean value that indicates whether a user enabled Studio Light on a device.

