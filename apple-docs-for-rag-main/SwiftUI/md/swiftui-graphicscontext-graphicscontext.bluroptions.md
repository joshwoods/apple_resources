

- SwiftUI
- GraphicsContext
-  GraphicsContext.BlurOptions 

Structure

# GraphicsContext.BlurOptions

Options that configure the graphics context filter that creates blur.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct BlurOptions
```

## Overview

You can use a set of these options when you call blur(radius:options:) to create a GraphicsContext.Filter that adds blur to an object that you draw into a GraphicsContext.

## Topics

### Getting blur options

static var dithersResult: GraphicsContext.BlurOptions

An option that causes the filter to dither the result, to reduce banding.

static var opaque: GraphicsContext.BlurOptions

An option that causes the filter to ensure the result is completely opaque.

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

struct ShadowOptions

Options that configure the graphics context filter that creates shadows.

