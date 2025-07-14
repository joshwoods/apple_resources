

- SwiftUI
- Color
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the color by feeding them into the given hash function.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func hash(into hasher: inout Hasher)
```

## Parameters 

`hasher`  

The hash function to use when combining the components of the color.

## See Also

### Comparing colors

static func == (Color, Color) -> Bool

Indicates whether two colors are equal.

