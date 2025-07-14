

- ARKit
- ARBodyAnchor
-  estimatedScaleFactor 

Instance Property

# estimatedScaleFactor

A factor that relates the body’s default height with the height ARKit estimates at runtime.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var estimatedScaleFactor: CGFloat { get }
```

## Discussion

The default value is 1.0. If you set automaticSkeletonScaleEstimationEnabled to true on ARBodyTrackingConfiguration, ARKit sets this property to a value between 0.0 and 1.0.

ARKit must know the height of a person in the camera feed to estimate an accurate world position for the person’s body anchor. ARKit uses the value of estimatedScaleFactor to correct the body anchor’s position in the physical environment.

The default body is 1.8 meters tall.

