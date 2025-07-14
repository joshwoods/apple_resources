

- UIKit
- UIPointerStyle
-  hidden() 

Type Method

# hidden()

Hides the pointer when it moves over the current region.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
class func hidden() -> Self
```

## See Also

### Creating a pointer style

convenience init(effect: UIPointerEffect, shape: UIPointerShape?)

Applies the provided content effect and pointer shape to the current region.

convenience init(shape: UIPointerShape, constrainedAxes: UIAxis)

Morphs the pointer into the provided shape when hovering over the current region.

class func system() -> Self

Morphs the pointer into a default system-style pointer.

