

- SwiftUI
- Font
-  custom(\_:fixedSize:) 

Type Method

# custom(\_:fixedSize:)

Create a custom font with the given `name` and a fixed `size` that does not scale with Dynamic Type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func custom(
    _ name: String,
    fixedSize: CGFloat
) -> Font
```

## See Also

### Creating custom fonts

static func custom(String, size: CGFloat, relativeTo: Font.TextStyle) -> Font

Create a custom font with the given `name` and `size` that scales relative to the given `textStyle`.

static func custom(String, size: CGFloat) -> Font

Create a custom font with the given `name` and `size` that scales with the body text style.

