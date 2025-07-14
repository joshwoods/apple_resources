

- SwiftUI
- GraphicsContext
-  GraphicsContext.ClipOptions 

Structure

# GraphicsContext.ClipOptions

Options that affect the use of clip shapes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct ClipOptions
```

## Overview

Use these options to affect how SwiftUI interprets a clip shape when you call clip(to:style:options:) to add a path to the array of clip shapes, or when you call clipToLayer(opacity:options:content:) to add a clipping layer.

## Topics

### Getting clip options

static var inverse: GraphicsContext.ClipOptions

An option to invert the shape or layer alpha as the clip mask.

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

### Masking

func clip(to: Path, style: FillStyle, options: GraphicsContext.ClipOptions)

Adds a path to the context’s array of clip shapes.

func clipToLayer(opacity: Double, options: GraphicsContext.ClipOptions, content: (inout GraphicsContext) throws -> Void) rethrows

Adds a clip shape that you define in a new layer to the context’s array of clip shapes.

var clipBoundingRect: CGRect

The bounding rectangle of the intersection of all current clip shapes in the current user space.

