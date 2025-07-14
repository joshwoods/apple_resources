

- SwiftUI
- Image
-  Image.Interpolation 

Enumeration

# Image.Interpolation

The level of quality for rendering an image that requires interpolation, such as a scaled image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Interpolation
```

## Overview

The interpolation(_:) modifier specifies the interpolation behavior when using the resizable(capInsets:resizingMode:) modifier on an Image. Use this behavior to prioritize rendering performance or image quality.

## Topics

### Getting interpolation options

case high

A value that indicates a high level of interpolation quality, which may slow down image rendering.

case low

A value that indicates a low level of interpolation quality, which may speed up image rendering.

case medium

A value that indicates a medium level of interpolation quality, between the low- and high-quality values.

case none

A value that indicates SwiftUI doesn’t interpolate image data.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Specifying rendering behavior

func antialiased(Bool) -> Image

Specifies whether SwiftUI applies antialiasing when rendering the image.

func symbolRenderingMode(SymbolRenderingMode?) -> Image

Sets the rendering mode for symbol images within this view.

func renderingMode(Image.TemplateRenderingMode?) -> Image

Indicates whether SwiftUI renders an image as-is, or by using a different mode.

func interpolation(Image.Interpolation) -> Image

Specifies the current level of quality for rendering an image that requires interpolation.

enum TemplateRenderingMode

A type that indicates how SwiftUI renders images.

