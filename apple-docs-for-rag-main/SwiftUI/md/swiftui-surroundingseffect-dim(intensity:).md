

- SwiftUI
- SurroundingsEffect
-  dim(intensity:) 

Type Method

# dim(intensity:)

An effect that dims the passthrough video a custom amount.

visionOS 2.0+

``` source
static func dim(intensity: Double) -> SurroundingsEffect
```

## Discussion

Use this with the preferredSurroundingsEffect(_:) view modifier when you want to darken the passthrough while displaying a particular view. The value will be clamped between 0 and 1. This effect will only be applied while an immersive space is opened.

