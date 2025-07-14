

- SwiftUI
- GraphicsContext
-  GraphicsContext.GradientOptions 

Structure

# GraphicsContext.GradientOptions

Options that affect the rendering of color gradients.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct GradientOptions
```

## Overview

Use these options to affect how SwiftUI manages a gradient that you create for a GraphicsContext.Shading instance for use in a GraphicsContext.

## Topics

### Getting gradient options

static var linearColor: GraphicsContext.GradientOptions

An option that interpolates between colors in a linear color space.

static var mirror: GraphicsContext.GradientOptions

An option that repeats the gradient outside its nominal range, reflecting every other instance.

static var `repeat`: GraphicsContext.GradientOptions

An option that repeats the gradient outside its nominal range.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Drawing a path

func stroke(Path, with: GraphicsContext.Shading, lineWidth: CGFloat)

Draws a path into the context with a specified line width.

func stroke(Path, with: GraphicsContext.Shading, style: StrokeStyle)

Draws a path into the context with a specified stroke style.

func fill(Path, with: GraphicsContext.Shading, style: FillStyle)

Draws a path into the context and fills the outlined region.

struct Shading

A color or pattern that you can use to outline or fill a path.

