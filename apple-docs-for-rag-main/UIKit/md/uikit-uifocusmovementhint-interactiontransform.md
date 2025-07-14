

- UIKit
- UIFocusMovementHint
-  interactionTransform 

Instance Property

# interactionTransform

A 3D transform that contains the combined transformations of perspective, rotation, and translation.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
var interactionTransform: CATransform3D { get }
```

## See Also

### Transforming a hint

var perspectiveTransform: CATransform3D

A 3D transform that represents a perspective matrix to be applied to match UIKit interaction hinting.

var rotation: CGVector

A vector to apply to a transform to match system interaction hinting.

var translation: CGVector

A vector to apply to a transform to match system interaction hinting.

