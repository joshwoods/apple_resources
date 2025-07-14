

- UIKit
- UIPointerStyle
-  init(effect:shape:) 

Initializer

# init(effect:shape:)

Applies the provided content effect and pointer shape to the current region.

iOS 13.4+iPadOS 13.4+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
convenience init(
    effect: UIPointerEffect,
    shape: UIPointerShape? = nil
)
```

## Parameters 

`effect`  

The UIPointerEffect to apply to the region.

`shape`  

The UIPointerShape to use, defaults to `nil`.

## See Also

### Creating a pointer style

convenience init(shape: UIPointerShape, constrainedAxes: UIAxis)

Morphs the pointer into the provided shape when hovering over the current region.

class func hidden() -> Self

Hides the pointer when it moves over the current region.

class func system() -> Self

Morphs the pointer into a default system-style pointer.

