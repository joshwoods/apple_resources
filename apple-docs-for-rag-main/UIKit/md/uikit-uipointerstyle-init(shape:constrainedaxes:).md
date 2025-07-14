

- UIKit
- UIPointerStyle
-  init(shape:constrainedAxes:) 

Initializer

# init(shape:constrainedAxes:)

Morphs the pointer into the provided shape when hovering over the current region.

iOS 13.4+iPadOS 13.4+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
convenience init(
    shape: UIPointerShape,
    constrainedAxes: UIAxis = []
)
```

## Parameters 

`shape`  

The UIPointerShape to use, defaults to `nil`.

`constrainedAxes`  

An array of UIAxis directions in which to constrain the pointer. The default is no constraints.

## See Also

### Creating a pointer style

convenience init(effect: UIPointerEffect, shape: UIPointerShape?)

Applies the provided content effect and pointer shape to the current region.

class func hidden() -> Self

Hides the pointer when it moves over the current region.

class func system() -> Self

Morphs the pointer into a default system-style pointer.

