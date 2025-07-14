

- SwiftUI
- Font
-  system(\_:design:weight:) 

Type Method

# system(\_:design:weight:)

Gets a system font that uses the specified style, design, and weight.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func system(
    _ style: Font.TextStyle,
    design: Font.Design? = nil,
    weight: Font.Weight? = nil
) -> Font
```

## Discussion

Use this method to create a system font that has the specified properties. The following example creates a system font with the Font.TextStyle.body text style, a Font.Design.serif design, and a bold weight, and applies the font to a Text view using the font(_:) view modifier:

```
Text("Hello").font(.system(.body, design: .serif, weight: .bold))
```

The `design` and `weight` parameters are both optional. If you omit either, the system uses a default value for that parameter. The default values are typically Font.Design.default and regular, respectively, but might vary depending on the context.

## See Also

### Getting system fonts

static func system(size: CGFloat, weight: Font.Weight?, design: Font.Design?) -> Font

Specifies a system font to use, along with the style, weight, and any design parameters you want applied to the text.

enum Design

A design to use for fonts.

enum TextStyle

A dynamic text style to use for fonts.

struct Weight

A weight to use for fonts.

