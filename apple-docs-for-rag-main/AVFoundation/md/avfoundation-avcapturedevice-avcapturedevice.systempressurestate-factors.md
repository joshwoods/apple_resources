

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.SystemPressureState
-  factors 

Instance Property

# factors

The set of underlying causes for the system pressure level.

iOS 11.1+iPadOS 11.1+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
var factors: AVCaptureDevice.SystemPressureState.Factors { get }
```

## Discussion

Increased system pressure may be due to one or more contributing causes; this set provides additional details for the overall performance characterization reported by the level property.

When the system pressure level is high, you can use this information to choose how to mitigate the issue. For example, you can reduce high system pressure due to depthModuleTemperature (on a builtInTrueDepthCamera device) by limiting the depth capture frame rate.

## See Also

### Contributing Factors

struct Factors

A structure that defines the factors affecting capture system performance.

