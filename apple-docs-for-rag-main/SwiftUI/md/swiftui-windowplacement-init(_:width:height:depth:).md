

- SwiftUI
- WindowPlacement
-  init(\_:width:height:depth:) 

Initializer

# init(\_:width:height:depth:)

Creates a new window placement with an optional position and 3D size. Depth is ignored on scenes or platforms that don’t support it.

visionOS 2.0+

``` source
init(
    _ position: WindowPlacement.Position? = nil,
    width: CGFloat? = nil,
    height: CGFloat? = nil,
    depth: CGFloat? = nil
)
```

## Discussion

Any values not provided will use use the default values for the `Scene` that this placement is being applied to.

