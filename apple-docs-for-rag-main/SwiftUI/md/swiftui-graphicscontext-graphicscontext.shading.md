

- SwiftUI
- GraphicsContext
-  GraphicsContext.Shading 

Structure

# GraphicsContext.Shading

A color or pattern that you can use to outline or fill a path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Shading
```

## Overview

Use a shading instance to describe the color or pattern of a path that you outline with a method like stroke(_:with:style:), or of the interior of a region that you fill with the fill(_:with:style:) method. Get a shading instance by calling one of the `Shading` structure’s factory methods. You can base shading on:

- A Color.

- A Gradient.

- Any type that conforms to ShapeStyle.

- An Image.

- What you’ve already drawn into the context.

- A collection of other shading instances.

## Topics

### Colors

static func color(Color) -> GraphicsContext.Shading

Returns a shading instance that fills with a color.

static func color(Color.RGBColorSpace, red: Double, green: Double, blue: Double, opacity: Double) -> GraphicsContext.Shading

Returns a shading instance that fills with a color in the given color space.

static func color(Color.RGBColorSpace, white: Double, opacity: Double) -> GraphicsContext.Shading

Returns a shading instance that fills with a monochrome color in the given color space.

### Gradients

static func linearGradient(Gradient, startPoint: CGPoint, endPoint: CGPoint, options: GraphicsContext.GradientOptions) -> GraphicsContext.Shading

Returns a shading instance that fills a linear (axial) gradient.

static func radialGradient(Gradient, center: CGPoint, startRadius: CGFloat, endRadius: CGFloat, options: GraphicsContext.GradientOptions) -> GraphicsContext.Shading

Returns a shading instance that fills a radial gradient.

static func conicGradient(Gradient, center: CGPoint, angle: Angle, options: GraphicsContext.GradientOptions) -> GraphicsContext.Shading

Returns a shading instance that fills a conic (angular) gradient.

### Other shape styles

static func style&lt;S>(S) -> GraphicsContext.Shading

Returns a shading instance that fills with the given shape style.

static var foreground: GraphicsContext.Shading

A shading instance that fills with the foreground style from the graphics context’s environment.

### Images

static func tiledImage(Image, origin: CGPoint, sourceRect: CGRect, scale: CGFloat) -> GraphicsContext.Shading

Returns a shading instance that tiles an image across the infinite plane.

### Composite shading types

static func palette([GraphicsContext.Shading]) -> GraphicsContext.Shading

Returns a multilevel shading instance constructed from an array of shading instances.

static var backdrop: GraphicsContext.Shading

A shading instance that draws a copy of the current background.

### Using a custom Metal shader

static func shader(Shader, bounds: CGRect) -> GraphicsContext.Shading

Returns a shading instance that fills with the results of querying a shader for each pixel.

### Type Methods

static func meshGradient(MeshGradient) -> GraphicsContext.Shading

Returns a shading instance that fills with a mesh gradient.

## Relationships

### Conforms To

- Sendable

## See Also

### Drawing a path

func stroke(Path, with: GraphicsContext.Shading, lineWidth: CGFloat)

Draws a path into the context with a specified line width.

func stroke(Path, with: GraphicsContext.Shading, style: StrokeStyle)

Draws a path into the context with a specified stroke style.

func fill(Path, with: GraphicsContext.Shading, style: FillStyle)

Draws a path into the context and fills the outlined region.

struct GradientOptions

Options that affect the rendering of color gradients.

