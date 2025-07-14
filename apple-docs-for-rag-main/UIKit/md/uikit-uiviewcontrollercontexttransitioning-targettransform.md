

- UIKit
- UIViewControllerContextTransitioning
-  targetTransform 

Instance Property

# targetTransform

Returns a transform indicating the amount of rotation being applied during the transition.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var targetTransform: CGAffineTransform { get }
```

**Required**

## Return Value

An affine transform indicating the amount of rotation being applied to the interface. This transform is the identity transform when no rotation is applied; otherwise, it is a transform that applies a 90 degree, -90 degree, or 180 degree rotation.

