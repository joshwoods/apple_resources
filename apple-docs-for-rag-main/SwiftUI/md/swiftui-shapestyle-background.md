

- SwiftUI
- ShapeStyle
-  background 

Type Property

# background

The background style in the current context.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var background: BackgroundStyle { get }
```

Available when `Self` is `BackgroundStyle`.

## Discussion

Access this value to get the style SwiftUI uses for the background in the current context. The specific color that SwiftUI renders depends on factors like the platform and whether the user has turned on Dark Mode.

For information about how to use shape styles, see ShapeStyle.

## See Also

### Semantic styles

static var foreground: ForegroundStyle

The foreground style in the current context.

static var selection: SelectionShapeStyle

A style used to visually indicate selection following platform conventional colors and behaviors.

static var separator: SeparatorShapeStyle

A style appropriate for foreground separator or border lines.

static var tint: TintShapeStyle

A style that reflects the current tint color.

static var placeholder: PlaceholderTextShapeStyle

A style appropriate for placeholder text.

static var link: LinkShapeStyle

A style appropriate for links.

static var fill: FillShapeStyle

An overlay fill style for filling shapes.

static var windowBackground: WindowBackgroundShapeStyle

A style appropriate for elements that should match the background of their containing window.

