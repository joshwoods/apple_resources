

- SwiftUI
- GraphicsContext
-  GraphicsContext.ShadowOptions 

Structure

# GraphicsContext.ShadowOptions

Options that configure the graphics context filter that creates shadows.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct ShadowOptions
```

## Overview

You can use a set of these options when you call shadow(color:radius:x:y:blendMode:options:) to create a GraphicsContext.Filter that adds a drop shadow to an object that you draw into a GraphicsContext.

## Topics

### Getting shadow options

static var disablesGroup: GraphicsContext.ShadowOptions

An option that causes the filter to composite the object and its shadow separately in the current layer.

static var invertsAlpha: GraphicsContext.ShadowOptions

An option that causes the filter to invert the alpha of the shadow.

static var shadowAbove: GraphicsContext.ShadowOptions

An option that causes the filter to draw the shadow above the object, rather than below it.

static var shadowOnly: GraphicsContext.ShadowOptions

An option that causes the filter to draw only the shadow, and omit the source object.

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

### Filtering

func addFilter(GraphicsContext.Filter, options: GraphicsContext.FilterOptions)

Adds a filter that applies to subsequent drawing operations.

struct Filter

A type that applies image processing operations to rendered content.

struct FilterOptions

Options that configure a filter that you add to a graphics context.

struct BlurOptions

Options that configure the graphics context filter that creates blur.

