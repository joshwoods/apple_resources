

- SwiftUI
- Font
-  system(size:weight:design:) 

Type Method

# system(size:weight:design:)

Specifies a system font to use, along with the style, weight, and any design parameters you want applied to the text.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func system(
    size: CGFloat,
    weight: Font.Weight? = nil,
    design: Font.Design? = nil
) -> Font
```

Show all declarations

## Discussion

Use this function to create a system font by specifying the size and weight, and a type design together. The following styles the system font as 17 point, semibold text:

```
Text("Hello").font(.system(size: 17, weight: .semibold))
```

While the following styles the text as 17 point bold, and applies a `serif` Font.Design to the system font:

```
Text("Hello").font(.system(size: 17, weight: .bold, design: .serif))
```

Both `weight` and `design` can be optional. When you do not provide a `weight` or `design`, the system can pick one based on the current context, which may not be regular or Font.Design.default in certain context. The following example styles the text as 17 point system font using Font.Design.rounded design, while its weight can depend on the current context:

```
Text("Hello").font(.system(size: 17, design: .rounded))
```

## See Also

### Getting system fonts

static func system(Font.TextStyle, design: Font.Design?, weight: Font.Weight?) -> Font

Gets a system font that uses the specified style, design, and weight.

enum Design

A design to use for fonts.

enum TextStyle

A dynamic text style to use for fonts.

struct Weight

A weight to use for fonts.

