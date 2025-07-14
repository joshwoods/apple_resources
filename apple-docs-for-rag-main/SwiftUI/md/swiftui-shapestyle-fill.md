

- SwiftUI
- ShapeStyle
-  fill 

Type Property

# fill

An overlay fill style for filling shapes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var fill: FillShapeStyle { get }
```

Available when `Self` is `FillShapeStyle`.

## Discussion

This shape style is appropriate for items situated on top of an existing background color. It incorporates transparency to allow the background color to show through.

Use the primary version of this style to fill thin or small shapes, such as the track of a slider on iOS. Use the secondary version of this style to fill medium-size shapes, such as the background of a switch on iOS. Use the tertiary version of this style to fill large shapes, such as input fields, search bars, or buttons on iOS. Use the quaternary version of this style to fill large areas that contain complex content, such as an expanded table cell on iOS.

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

static var windowBackground: WindowBackgroundShapeStyle

A style appropriate for elements that should match the background of their containing window.

