

- SwiftUI
- Font
-  system(size:weight:design:) Deprecated

Type Method

# system(size:weight:design:)

Specifies a system font to use, along with the style, weight, and any design parameters you want applied to the text.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
static func system(
    size: CGFloat,
    weight: Font.Weight = .regular,
    design: Font.Design = .default
) -> Font
```

Deprecated

Use system(size:weight:design:) instead.

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

If you want to use the default Font.Weight (regular), you don’t need to specify the `weight` in the method. The following example styles the text as 17 point regular, and uses a Font.Design.rounded system font:

```
Text("Hello").font(.system(size: 17, design: .rounded))
```

## See Also

### Deprecated symbols

static func system(Font.TextStyle, design: Font.Design) -> Font

Gets a system font with the given text style and design.

Deprecated

