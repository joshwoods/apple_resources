

- SwiftUI
-  Material 

Structure

# Material

A background material type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Material
```

## Overview

You can apply a blur effect to a view that appears behind another view by adding a material with the background(_:ignoresSafeAreaEdges:) modifier:

```
ZStack {
    Color.teal
    Label("Flag", systemImage: "flag.fill")
        .padding()
        .background(.regularMaterial)
}
```

In the example above, the ZStack layers a Label on top of the color teal. The background modifier inserts the regular material below the label, blurring the part of the background that the label — including its padding — covers:

A material isn’t a view, but adding a material is like inserting a translucent layer between the modified view and its background:

The blurring effect provided by the material isn’t simple opacity. Instead, it uses a platform-specific blending that produces an effect that resembles heavily frosted glass. You can see this more easily with a complex background, like an image:

```
ZStack {
    Image("chili_peppers")
        .resizable()
        .aspectRatio(contentMode: .fit)
    Label("Flag", systemImage: "flag.fill")
        .padding()
        .background(.regularMaterial)
}
```

For physical materials, the degree to which the background colors pass through depends on the thickness. The effect also varies with light and dark appearance:

If you need a material to have a particular shape, you can use the background(_:in:fillStyle:) modifier. For example, you can create a material with rounded corners:

```
ZStack {
    Color.teal
    Label("Flag", systemImage: "flag.fill")
        .padding()
        .background(.regularMaterial, in: RoundedRectangle(cornerRadius: 8))
}
```

When you add a material, foreground elements exhibit vibrancy, a context-specific blend of the foreground and background colors that improves contrast. However using foregroundStyle(_:) to set a custom foreground style — excluding the hierarchical styles, like secondary — disables vibrancy.

Note

A material blurs a background that’s part of your app, but not what appears behind your app on the screen. For example, the content on the Home Screen doesn’t affect the appearance of a widget.

## Topics

### Getting material types

static let ultraThin: Material

A mostly translucent material.

static let thin: Material

A material that’s more translucent than opaque.

static let regular: Material

A material that’s somewhat translucent.

static let thick: Material

A material that’s more opaque than translucent.

static let ultraThick: Material

A mostly opaque material.

static let bar: Material

A material matching the style of system toolbars.

### Instance Methods

func materialActiveAppearance(MaterialActiveAppearance) -> Material

Sets an explicit active appearance for this material.

## Relationships

### Conforms To

- Copyable
- Sendable
- ShapeStyle

## See Also

### Supporting types

struct AngularGradient

An angular gradient.

struct EllipticalGradient

A radial gradient that draws an ellipse.

struct LinearGradient

A linear gradient.

struct RadialGradient

A radial gradient.

struct ImagePaint

A shape style that fills a shape by repeating a region of an image.

struct HierarchicalShapeStyle

A shape style that maps to one of the numbered content styles.

struct HierarchicalShapeStyleModifier

Styles that you can apply to hierarchical shapes.

struct ForegroundStyle

The foreground style in the current context.

struct BackgroundStyle

The background style in the current context.

struct SelectionShapeStyle

A style used to visually indicate selection following platform conventional colors and behaviors.

struct SeparatorShapeStyle

A style appropriate for foreground separator or border lines.

struct TintShapeStyle

A style that reflects the current tint color.

struct FillShapeStyle

A shape style that displays one of the overlay fills.

struct LinkShapeStyle

A style appropriate for links.

struct PlaceholderTextShapeStyle

A style appropriate for placeholder text.

