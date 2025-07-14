

- UIKit
- UIMotionEffectGroup
-  motionEffects 

Instance Property

# motionEffects

An array of motion effect objects to apply as a group to the view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var motionEffects: [UIMotionEffect]? { get set }
```

## Discussion

The array contains one or more UIMotionEffect objects. When the viewer offset changes, each object in the group is asked for its key paths and updated values. Those values are then applied simultaneously.

