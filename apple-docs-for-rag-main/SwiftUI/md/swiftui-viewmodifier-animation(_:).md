

- SwiftUI
- ViewModifier
-  animation(\_:) 

Instance Method

# animation(\_:)

Returns a new version of the modifier that will apply `animation` to all animatable values within the modifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
func animation(_ animation: Animation?) -> some ViewModifier
```

## See Also

### Adding animations to a view

func concat&lt;T>(T) -> ModifiedContent&lt;Self, T>

Returns a new modifier that is the result of concatenating `self` with `modifier`.

