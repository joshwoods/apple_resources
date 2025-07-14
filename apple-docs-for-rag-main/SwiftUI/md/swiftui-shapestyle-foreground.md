

- SwiftUI
- ShapeStyle
-  foreground 

Type Property

# foreground

The foreground style in the current context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var foreground: ForegroundStyle { get }
```

Available when `Self` is `ForegroundStyle`.

## Discussion

Access this value to get the style SwiftUI uses for foreground elements, like text, symbols, and shapes, in the current context. Use the foregroundStyle(_:) modifier to set a new foreground style for a given view and its child views.

For information about how to use shape styles, see ShapeStyle.

## See Also

### Semantic styles

static var background: BackgroundStyle

The background style in the current context.

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

