

- SwiftUI
- WindowPlacement
-  init(\_:width:height:) 

Initializer

# init(\_:width:height:)

Creates a new window placement with a display-relative position, with an optional width and height.

macOS 15.0+

``` source
init(
    _ position: UnitPoint,
    width: CGFloat? = nil,
    height: CGFloat? = nil
)
```

## Discussion

Any values not provided will use use the default values for the `Scene` that this placement is being applied to.

