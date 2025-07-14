

- SwiftUI
-  ShapeStyle 

Protocol

# ShapeStyle

A color or pattern to use when rendering a shape.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol ShapeStyle : Sendable
```

## Overview

You create custom shape styles by declaring a type that conforms to the `ShapeStyle` protocol and implementing the required `resolve` function to return a shape style that represents the desired appearance based on the current environment.

For example this shape style reads the current color scheme from the environment to choose the blend mode its color will be composited with:

```
struct MyShapeStyle: ShapeStyle {
    func resolve(in environment: EnvironmentValues) -> some ShapeStyle {
        if environment.colorScheme == .light {
            return Color.red.blendMode(.lighten)
        } else {
            return Color.red.blendMode(.darken)
        }
    }
}
```

In addition to creating a custom shape style, you can also use one of the concrete styles that SwiftUI defines. To indicate a specific color or pattern, you can use Color or the style returned by image(_:sourceRect:scale:), or one of the gradient types, like the one returned by radialGradient(_:center:startRadius:endRadius:). To set a color that’s appropriate for a given context on a given platform, use one of the semantic styles, like background or primary.

You can use a shape style by:

- Filling a shape with a style with the fill(_:style:) modifier:

  ```
  Path { path in
      path.move(to: .zero)
      path.addLine(to: CGPoint(x: 50, y: 0))
      path.addArc(
          center: .zero,
          radius: 50,
          startAngle: .zero,
          endAngle: .degrees(90),
          clockwise: false)
  }
  .fill(.radialGradient(
      Gradient(colors: [.yellow, .red]),
      center: .topLeading,
      startRadius: 15,
      endRadius: 80))
  ```

- Tracing the outline of a shape with a style with either the stroke(_:lineWidth:) or the stroke(_:style:) modifier:

  ```
  RoundedRectangle(cornerRadius: 10)
      .stroke(.mint, lineWidth: 10)
      .frame(width: 200, height: 50)
  ```

- Styling the foreground elements in a view with the foregroundStyle(_:) modifier:

  ```
  VStack(alignment: .leading) {
      Text("Primary")
          .font(.title)
      Text("Secondary")
          .font(.caption)
          .foregroundStyle(.secondary)
  }
  ```

## Topics

### System colors

static var black: Color

A black color suitable for use in UI elements.

static var blue: Color

A context-dependent blue color suitable for use in UI elements.

static var brown: Color

A context-dependent brown color suitable for use in UI elements.

static var clear: Color

A clear color suitable for use in UI elements.

static var cyan: Color

A context-dependent cyan color suitable for use in UI elements.

static var gray: Color

A context-dependent gray color suitable for use in UI elements.

static var green: Color

A context-dependent green color suitable for use in UI elements.

static var indigo: Color

A context-dependent indigo color suitable for use in UI elements.

static var mint: Color

A context-dependent mint color suitable for use in UI elements.

static var orange: Color

A context-dependent orange color suitable for use in UI elements.

static var pink: Color

A context-dependent pink color suitable for use in UI elements.

static var purple: Color

A context-dependent purple color suitable for use in UI elements.

static var red: Color

A context-dependent red color suitable for use in UI elements.

static var teal: Color

A context-dependent teal color suitable for use in UI elements.

static var white: Color

A white color suitable for use in UI elements.

static var yellow: Color

A context-dependent yellow color suitable for use in UI elements.

### Angular gradients

static angularGradient(_:center:startAngle:endAngle:)

An angular gradient, which applies the color function as the angle changes between the start and end angles, and anchored to a relative center point within the filled shape.

static func angularGradient(colors: [Color], center: UnitPoint, startAngle: Angle, endAngle: Angle) -> AngularGradient

An angular gradient defined by a collection of colors.

static func angularGradient(stops: [Gradient.Stop], center: UnitPoint, startAngle: Angle, endAngle: Angle) -> AngularGradient

An angular gradient defined by a collection of color stops.

### Conic gradients

static conicGradient(_:center:angle:)

A conic gradient that completes a full turn, optionally starting from a given angle and anchored to a relative center point within the filled shape.

static func conicGradient(colors: [Color], center: UnitPoint, angle: Angle) -> AngularGradient

A conic gradient defined by a collection of colors that completes a full turn.

static func conicGradient(stops: [Gradient.Stop], center: UnitPoint, angle: Angle) -> AngularGradient

A conic gradient defined by a collection of color stops that completes a full turn.

### Elliptical gradients

static ellipticalGradient(_:center:startRadiusFraction:endRadiusFraction:)

A radial gradient that draws an ellipse.

static func ellipticalGradient(colors: [Color], center: UnitPoint, startRadiusFraction: CGFloat, endRadiusFraction: CGFloat) -> EllipticalGradient

A radial gradient that draws an ellipse defined by a collection of colors.

static func ellipticalGradient(stops: [Gradient.Stop], center: UnitPoint, startRadiusFraction: CGFloat, endRadiusFraction: CGFloat) -> EllipticalGradient

A radial gradient that draws an ellipse defined by a collection of color stops.

### Linear gradients

static linearGradient(_:startPoint:endPoint:)

A linear gradient.

static func linearGradient(colors: [Color], startPoint: UnitPoint, endPoint: UnitPoint) -> LinearGradient

A linear gradient defined by a collection of colors.

static func linearGradient(stops: [Gradient.Stop], startPoint: UnitPoint, endPoint: UnitPoint) -> LinearGradient

A linear gradient defined by a collection of color stops.

### Radial gradients

static radialGradient(_:center:startRadius:endRadius:)

A radial gradient.

static func radialGradient(colors: [Color], center: UnitPoint, startRadius: CGFloat, endRadius: CGFloat) -> RadialGradient

A radial gradient defined by a collection of colors.

static func radialGradient(stops: [Gradient.Stop], center: UnitPoint, startRadius: CGFloat, endRadius: CGFloat) -> RadialGradient

A radial gradient defined by a collection of color stops.

### Materials

static var ultraThinMaterial: Material

A mostly translucent material.

static var thinMaterial: Material

A material that’s more translucent than opaque.

static var regularMaterial: Material

A material that’s somewhat translucent.

static var thickMaterial: Material

A material that’s more opaque than translucent.

static var ultraThickMaterial: Material

A mostly opaque material.

static var bar: Material

A material matching the style of system toolbars.

### Image paint styles

static func image(Image, sourceRect: CGRect, scale: CGFloat) -> ImagePaint

A shape style that fills a shape by repeating a region of an image.

### Hierarchical styles

var secondary: some ShapeStyle

Returns the second level of this shape style.

var tertiary: some ShapeStyle

Returns the third level of this shape style.

var quaternary: some ShapeStyle

Returns the fourth level of this shape style.

var quinary: some ShapeStyle

Returns the fifth level of this shape style.

static var primary: HierarchicalShapeStyle

A shape style that maps to the first level of the current content style.

static var secondary: HierarchicalShapeStyle

A shape style that maps to the second level of the current content style.

static var tertiary: HierarchicalShapeStyle

A shape style that maps to the third level of the current content style.

static var quaternary: HierarchicalShapeStyle

A shape style that maps to the fourth level of the current content style.

static var quinary: HierarchicalShapeStyle

A shape style that maps to the fifth level of the current content style.

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

static var windowBackground: WindowBackgroundShapeStyle

A style appropriate for elements that should match the background of their containing window.

### Modifying a shape style

func blendMode(BlendMode) -> some ShapeStyle

Returns a new style based on `self` that applies the specified blend mode when drawing.

func opacity(Double) -> some ShapeStyle

Returns a new style based on `self` that multiplies by the specified opacity when drawing.

func shadow(ShadowStyle) -> some ShapeStyle

Applies the specified shadow effect to the shape style.

### Configuring the default shape style

static func blendMode(BlendMode) -> some ShapeStyle

Returns a new style based on the current style that uses `mode` as its blend mode when drawing.

static func opacity(Double) -> some ShapeStyle

Returns a new style based on the current style that multiplies by `opacity` when drawing.

static func shadow(ShadowStyle) -> some ShapeStyle

Returns a shape style that applies the specified shadow style to the current style.

### Mapping to absolute coordinates

func `in`(CGRect) -> some ShapeStyle

Maps a shape style’s unit-space coordinates to the absolute coordinates of a given rectangle.

### Resolving a shape style in an environment

func resolve(in: EnvironmentValues) -> Self.Resolved

Evaluate to a resolved shape style given the current `environment`.

**Required** Default implementation provided.

associatedtype Resolved : ShapeStyle = Never

The type of shape style this will resolve to.

**Required**

### Using a shape style as a view

var body: _ShapeView&lt;Rectangle, Self>

A rectangular view that’s filled with the shape style.

### Supporting types

Construct instances of these styles using the properties and methods of the shape style protocol.

struct AngularGradient

An angular gradient.

struct EllipticalGradient

A radial gradient that draws an ellipse.

struct LinearGradient

A linear gradient.

struct RadialGradient

A radial gradient.

struct Material

A background material type.

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

struct WindowBackgroundShapeStyle

A style appropriate for elements that should match the background of their containing window.

### Instance Methods

func materialActiveAppearance(MaterialActiveAppearance) -> some ShapeStyle

Sets an explicit active appearance for materials created by this style.

## Relationships

### Inherits From

- Sendable

### Conforming Types

- AngularGradient
- AnyGradient
- AnyShapeStyle
- BackgroundStyle
- Color
- Color.Resolved
- EllipticalGradient
- FillShapeStyle
- ForegroundStyle
- Gradient
- HierarchicalShapeStyle
- HierarchicalShapeStyleModifier
- ImagePaint
- LinearGradient
- LinkShapeStyle
- Material
- MeshGradient
- PlaceholderTextShapeStyle
- RadialGradient
- SelectionShapeStyle
- SeparatorShapeStyle
- Shader
- TintShapeStyle
- WindowBackgroundShapeStyle

## See Also

### Styling content

func border&lt;S>(S, width: CGFloat) -> some View

Adds a border to this view with the specified style and width.

func foregroundStyle&lt;S>(S) -> some View

Sets a view’s foreground elements to use a given style.

func foregroundStyle&lt;S1, S2>(S1, S2) -> some View

Sets the primary and secondary levels of the foreground style in the child view.

func foregroundStyle&lt;S1, S2, S3>(S1, S2, S3) -> some View

Sets the primary, secondary, and tertiary levels of the foreground style.

func backgroundStyle&lt;S>(S) -> some View

Sets the specified style to render backgrounds within the view.

var backgroundStyle: AnyShapeStyle?

An optional style that overrides the default system background style when set.

struct AnyShapeStyle

A type-erased ShapeStyle value.

struct Gradient

A color gradient represented as an array of color stops, each having a parametric location value.

struct MeshGradient

A two-dimensional gradient defined by a 2D grid of positioned colors.

struct AnyGradient

A color gradient.

struct ShadowStyle

A style to use when rendering shadows.

