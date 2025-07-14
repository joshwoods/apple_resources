

- SwiftUI
- GraphicsContext
-  GraphicsContext.FilterOptions 

Structure

# GraphicsContext.FilterOptions

Options that configure a filter that you add to a graphics context.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct FilterOptions
```

## Overview

You can use filter options to configure a GraphicsContext.Filter that you apply to a GraphicsContext with the addFilter(_:options:) method.

## Topics

### Getting filter options

static var linearColor: GraphicsContext.FilterOptions

An option that causes the filter to perform calculations in a linear color space.

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

struct BlurOptions

Options that configure the graphics context filter that creates blur.

struct ShadowOptions

Options that configure the graphics context filter that creates shadows.

