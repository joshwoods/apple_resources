

- ARKit
- ARBodyTrackingConfiguration
-  automaticSkeletonScaleEstimationEnabled 

Instance Property

# automaticSkeletonScaleEstimationEnabled

A flag that determines whether ARKit estimates the height of a body that it’s tracking.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var automaticSkeletonScaleEstimationEnabled: Bool { get set }
```

## Discussion

When you assign this property a value of true, you instruct ARKit to compute a value for estimatedScaleFactor for a person’s body anchor. ARKit must know the physical height of a person in the real world to accurately estimate the person’s real-world position. You enable this property to tell ARKit to estimate a recognized person’s physical height before it assigns the body anchor’s position.

