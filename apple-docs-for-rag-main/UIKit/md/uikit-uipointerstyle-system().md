

- UIKit
- UIPointerStyle
-  system() 

Type Method

# system()

Morphs the pointer into a default system-style pointer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class func system() -> Self
```

## Discussion

To display custom accessories alongside the default pointer, use this pointer style and assign your accessories to the accessories property.

## See Also

### Creating a pointer style

convenience init(effect: UIPointerEffect, shape: UIPointerShape?)

Applies the provided content effect and pointer shape to the current region.

convenience init(shape: UIPointerShape, constrainedAxes: UIAxis)

Morphs the pointer into the provided shape when hovering over the current region.

class func hidden() -> Self

Hides the pointer when it moves over the current region.

