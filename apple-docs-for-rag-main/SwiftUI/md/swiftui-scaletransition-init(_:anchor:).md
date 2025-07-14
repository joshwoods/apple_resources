

- SwiftUI
- ScaleTransition
-  init(\_:anchor:) 

Initializer

# init(\_:anchor:)

Creates a transition that scales the view by the specified amount.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    _ scale: Double,
    anchor: UnitPoint = .center
)
```

## See Also

### Creating the transition

var anchor: UnitPoint

The anchor point to scale the view around.

var scale: Double

The amount to scale the view by.

