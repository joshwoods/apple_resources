

- UIKit
-  UIGraphicsImageRendererContext 

Class

# UIGraphicsImageRendererContext

The drawing environment for an image renderer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class UIGraphicsImageRendererContext
```

## Overview

When using the UIGraphicsImageRenderer drawing methods, you must pass a block of type UIGraphicsImageRenderer.DrawingActions as an argument, which provides a UIGraphicsImageRendererContext instance as an argument. Use the context object to access high-level drawing functions and the underlying Core Graphics context.

Note

`UIGraphicsImageRendererContext` inherits much of its functionality from its abstract superclass UIGraphicsRendererContext.

To learn how to use a `UIGraphicsImageRendererContext` object in combination with an image renderer, see Creating a graphics image renderer.

## Topics

### Getting the image

var currentImage: UIImage

The current state of the drawing context, expressed as an object that manages image data in your app.

### Getting the image drawing actions

typealias DrawingActions

A closure for drawing an image.

## Relationships

### Inherits From

- UIGraphicsRendererContext

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

class UIGraphicsRendererContext

The base class for the drawing environments for graphics renderers.

class UIGraphicsRendererFormat

A set of drawing attributes that represents the configuration of a graphics renderer context.

class UIGraphicsImageRenderer

A graphics renderer for creating Core Graphics-backed images.

class UIGraphicsImageRendererFormat

A set of drawing attributes that represents the configuration of an image renderer context.

class UIGraphicsPDFRenderer

A graphics renderer for creating PDFs.

class UIGraphicsPDFRendererContext

The drawing environment for a PDF renderer.

class UIGraphicsPDFRendererFormat

A set of drawing attributes that represents the configuration of a PDF renderer context.

