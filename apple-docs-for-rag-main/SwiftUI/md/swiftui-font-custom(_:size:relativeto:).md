

- SwiftUI
- Font
-  custom(\_:size:relativeTo:) 

Type Method

# custom(\_:size:relativeTo:)

Create a custom font with the given `name` and `size` that scales relative to the given `textStyle`.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func custom(
    _ name: String,
    size: CGFloat,
    relativeTo textStyle: Font.TextStyle
) -> Font
```

## See Also

### Creating custom fonts

static func custom(String, fixedSize: CGFloat) -> Font

Create a custom font with the given `name` and a fixed `size` that does not scale with Dynamic Type.

static func custom(String, size: CGFloat) -> Font

Create a custom font with the given `name` and `size` that scales with the body text style.

