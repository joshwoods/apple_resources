

- SwiftUI
- ShapeStyle
-  tint 

Type Property

# tint

A style that reflects the current tint color.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var tint: TintShapeStyle { get }
```

Available when `Self` is `TintShapeStyle`.

## Discussion

You can set the tint color with the `tint(_:)` modifier. If no explicit tint is set, the tint is derived from the app’s accent color.

## See Also

### Semantic styles

static var foreground: ForegroundStyle

The foreground style in the current context.

static var background: BackgroundStyle

The background style in the current context.

static var selection: SelectionShapeStyle

A style used to visually indicate selection following platform conventional colors and behaviors.

static var separator: SeparatorShapeStyle

A style appropriate for foreground separator or border lines.

static var placeholder: PlaceholderTextShapeStyle

A style appropriate for placeholder text.

static var link: LinkShapeStyle

A style appropriate for links.

static var fill: FillShapeStyle

An overlay fill style for filling shapes.

static var windowBackground: WindowBackgroundShapeStyle

A style appropriate for elements that should match the background of their containing window.

