

- UIKit
- UIFocusMovementHint
-  rotation 

Instance Property

# rotation

A vector to apply to a transform to match system interaction hinting.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
var rotation: CGVector { get }
```

## Discussion

This property represents an X,Y-axis translation expressed in radians.

## See Also

### Transforming a hint

var interactionTransform: CATransform3D

A 3D transform that contains the combined transformations of perspective, rotation, and translation.

var perspectiveTransform: CATransform3D

A 3D transform that represents a perspective matrix to be applied to match UIKit interaction hinting.

var translation: CGVector

A vector to apply to a transform to match system interaction hinting.

