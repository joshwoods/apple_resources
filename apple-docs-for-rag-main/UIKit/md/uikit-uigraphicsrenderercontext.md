

- UIKit
-  UIGraphicsRendererContext 

Class

# UIGraphicsRendererContext

The base class for the drawing environments for graphics renderers.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class UIGraphicsRendererContext
```

## Overview

You don’t create instances of UIGraphicsRendererContext yourself. Instead, when you use a concrete subclass of UIGraphicsRenderer, you are provided an instance of the appropriate UIGraphicsRendererContext subclass—either UIGraphicsImageRendererContext or UIGraphicsPDFRendererContext—as an argument to a UIGraphicsDrawingActions drawing actions block.

UIGraphicsRendererContext objects provide high-level drawing methods in addition to access to the underlying Core Graphics context.

## Topics

### Getting the drawing context

var cgContext: CGContext

The underlying Core Graphics context.

var format: UIGraphicsRendererFormat

The format used to create the associated graphics renderer.

### Drawing content

func stroke(CGRect)

Paints a rectangular path using the currently selected stroke color.

func stroke(CGRect, blendMode: CGBlendMode)

Paints a rectangular path using the currently selected stroke color and specified blend mode.

func fill(CGRect, blendMode: CGBlendMode)

Paints a rectangular area with the currently selected fill color using the supplied blend mode.

func fill(CGRect)

Paints a rectangular area with the currently selected fill color.

### Applying a clipping rectangle

func clip(to: CGRect)

Sets the clipping mask for the drawing context to the specified rectangle.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIGraphicsImageRendererContext
- UIGraphicsPDFRendererContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Graphics contexts

class UIGraphicsRenderer

An abstract base class for creating graphics renderers.

class UIGraphicsRendererFormat

A set of drawing attributes that represents the configuration of a graphics renderer context.

class UIGraphicsImageRenderer

A graphics renderer for creating Core Graphics-backed images.

class UIGraphicsImageRendererContext

The drawing environment for an image renderer.

class UIGraphicsImageRendererFormat

A set of drawing attributes that represents the configuration of an image renderer context.

class UIGraphicsPDFRenderer

A graphics renderer for creating PDFs.

class UIGraphicsPDFRendererContext

The drawing environment for a PDF renderer.

class UIGraphicsPDFRendererFormat

A set of drawing attributes that represents the configuration of a PDF renderer context.

