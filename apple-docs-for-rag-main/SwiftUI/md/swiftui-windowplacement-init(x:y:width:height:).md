

- SwiftUI
- WindowPlacement
-  init(x:y:width:height:) 

Initializer

# init(x:y:width:height:)

Creates a new window placement with an optional position and size.

macOS 15.0+

``` source
init(
    x: CGFloat? = nil,
    y: CGFloat? = nil,
    width: CGFloat? = nil,
    height: CGFloat? = nil
)
```

## Discussion

Any values not provided will use use the default values for the `Scene` that this placement is being applied to.

