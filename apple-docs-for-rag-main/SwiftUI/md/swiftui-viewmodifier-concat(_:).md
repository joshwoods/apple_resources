

- SwiftUI
- ViewModifier
-  concat(\_:) 

Instance Method

# concat(\_:)

Returns a new modifier that is the result of concatenating `self` with `modifier`.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func concat(_ modifier: T) -> ModifiedContent
```

## See Also

### Adding animations to a view

func animation(Animation?) -> some ViewModifier

Returns a new version of the modifier that will apply `animation` to all animatable values within the modifier.

