

- SwiftUI
- WindowPlacement
-  init(\_:size3D:) 

Initializer

# init(\_:size3D:)

Creates a new window placement with an optional position and 3D size. Depth is ignored on scenes that don’t support it.

visionOS 2.0+

``` source
init(
    _ position: WindowPlacement.Position? = nil,
    size3D: Size3D? = nil
)
```

## Discussion

Any values not provided will use use the default values for the `Scene` that this placement is being applied to.

