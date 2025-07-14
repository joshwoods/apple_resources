

- SwiftUI
- Font
-  custom(\_:size:) 

Type Method

# custom(\_:size:)

Create a custom font with the given `name` and `size` that scales with the body text style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func custom(
    _ name: String,
    size: CGFloat
) -> Font
```

## Mentioned in 

Applying custom fonts to text

## See Also

### Creating custom fonts

static func custom(String, fixedSize: CGFloat) -> Font

Create a custom font with the given `name` and a fixed `size` that does not scale with Dynamic Type.

static func custom(String, size: CGFloat, relativeTo: Font.TextStyle) -> Font

Create a custom font with the given `name` and `size` that scales relative to the given `textStyle`.

