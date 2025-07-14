

- SwiftUI
- ShapeStyle
-  windowBackground 

Type Property

# windowBackground

A style appropriate for elements that should match the background of their containing window.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
static var windowBackground: WindowBackgroundShapeStyle { get }
```

Available when `Self` is `WindowBackgroundShapeStyle`.

## Discussion

On macOS, this has a unique appearance compared to the default `ShapeStyle.background`. It matches the default background of a window: a wallpaper-tinted light gray in the light appearance and a wallpaper-tinted dark gray in the dark appearance.

On visionOS, the default glass window background can only be created using `glassBackgroundEffect`.

For information about how to use shape styles, see ShapeStyle.

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

static var tint: TintShapeStyle

A style that reflects the current tint color.

static var placeholder: PlaceholderTextShapeStyle

A style appropriate for placeholder text.

static var link: LinkShapeStyle

A style appropriate for links.

static var fill: FillShapeStyle

An overlay fill style for filling shapes.

