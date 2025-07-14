

- SwiftUI
- Color
-  gradient 

Instance Property

# gradient

Returns the standard gradient for the color `self`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var gradient: AnyGradient { get }
```

## Discussion

For example, filling a rectangle with a gradient derived from the standard blue color:

```
Rectangle().fill(.blue.gradient)
```

## See Also

### Modifying a color

func opacity(Double) -> Color

Multiplies the opacity of the color by the given amount.

