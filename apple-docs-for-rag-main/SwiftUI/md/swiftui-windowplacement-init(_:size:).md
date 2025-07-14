

- SwiftUI
- WindowPlacement
-  init(\_:size:) 

Initializer

# init(\_:size:)

Creates a new window placement with an absolute position and optional size.

macOS 15.0+

``` source
init(
    _ position: CGPoint? = nil,
    size: CGSize? = nil
)
```

Show all declarations

## Discussion

Any values not provided will use use the default values for the `Scene` that this placement is being applied to.

