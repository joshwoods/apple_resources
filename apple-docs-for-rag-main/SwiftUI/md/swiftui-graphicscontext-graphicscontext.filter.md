

- SwiftUI
- GraphicsContext
-  GraphicsContext.Filter 

Structure

# GraphicsContext.Filter

A type that applies image processing operations to rendered content.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Filter
```

## Overview

Create and configure a filter that produces an image processing effect, like adding a drop shadow or a blur effect, by calling one of the factory methods defined by the `Filter` structure. Call the addFilter(_:options:) method to add the filter to a GraphicsContext. The filter only affects content that you draw into the context after adding the filter.

## Topics

### Changing brightness and contrast

static func brightness(Double) -> GraphicsContext.Filter

Returns a filter that applies a brightness adjustment.

static func contrast(Double) -> GraphicsContext.Filter

Returns a filter that applies a contrast adjustment.

### Manipulating color

static func saturation(Double) -> GraphicsContext.Filter

Returns a filter that applies a saturation adjustment.

static func colorInvert(Double) -> GraphicsContext.Filter

Returns a filter that inverts the color of their results.

static func colorMultiply(Color) -> GraphicsContext.Filter

Returns a filter that multiplies each color component by the matching component of a given color.

static func hueRotation(Angle) -> GraphicsContext.Filter

Returns a filter that applies a hue rotation adjustment.

static func grayscale(Double) -> GraphicsContext.Filter

Returns a filter that applies a grayscale adjustment.

static func colorMatrix(ColorMatrix) -> GraphicsContext.Filter

Returns a filter that multiplies by a given color matrix.

### Adding blur

static func blur(radius: CGFloat, options: GraphicsContext.BlurOptions) -> GraphicsContext.Filter

Returns a filter that applies a Gaussian blur.

### Adding a shadow

static func shadow(color: Color, radius: CGFloat, x: CGFloat, y: CGFloat, blendMode: GraphicsContext.BlendMode, options: GraphicsContext.ShadowOptions) -> GraphicsContext.Filter

Returns a filter that adds a shadow.

### Adjusting opacity

static var luminanceToAlpha: GraphicsContext.Filter

Returns a filter that sets the opacity of each pixel based on its luminance.

static func alphaThreshold(min: Double, max: Double, color: Color) -> GraphicsContext.Filter

Returns a filter that replaces each pixel with alpha components within a range by a constant color, or transparency otherwise.

### Adding a transformation

static func projectionTransform(ProjectionTransform) -> GraphicsContext.Filter

Returns a filter that that transforms the rasterized form of subsequent graphics primitives.

### Using a custom Metal shader

static func colorShader(Shader) -> GraphicsContext.Filter

Returns a filter that applies `shader` to the color of each source pixel.

static func distortionShader(Shader, maxSampleOffset: CGSize) -> GraphicsContext.Filter

Returns a filter that applies `shader` as a geometric distortion effect on the location of each pixel.

static func layerShader(Shader, maxSampleOffset: CGSize) -> GraphicsContext.Filter

Returns a filter that applies `shader` to the contents of the source layer.

## Relationships

### Conforms To

- Sendable

## See Also

### Filtering

func addFilter(GraphicsContext.Filter, options: GraphicsContext.FilterOptions)

Adds a filter that applies to subsequent drawing operations.

struct FilterOptions

Options that configure a filter that you add to a graphics context.

struct BlurOptions

Options that configure the graphics context filter that creates blur.

struct ShadowOptions

Options that configure the graphics context filter that creates shadows.

