

- UIKit
-  UIGraphicsRendererFormat 

Class

# UIGraphicsRendererFormat

A set of drawing attributes that represents the configuration of a graphics renderer context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class UIGraphicsRendererFormat
```

## Overview

Create a UIGraphicsRendererFormat object, or one of its subclasses (UIGraphicsImageRendererFormat and UIGraphicsPDFRendererFormat), and use it to construct a graphics renderer by providing the format object as a parameter in a UIGraphicsRenderer subclass intializer.

The graphics renderer uses the format object you provided to configure any context objects (UIGraphicsRendererContext) it creates as part of the rendering process.

If you use a graphics renderer initializer that doesn’t require a format argument, the renderer creates a format object using the default() class method.

The renderer format object contains properties that represent the immutable aspects of the renderer’s configuration. This means that repeated uses of a single graphics renderer object will always use the same format object.

## Topics

### Creating a format

class func `default`() -> Self

Returns a format that represents the highest fidelity that the current device supports.

class func preferred() -> Self

Returns the most suitable format for the main screen’s current configuration.

### Getting the bounds

var bounds: CGRect

The bounds of the graphics context.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIGraphicsImageRendererFormat
- UIGraphicsPDFRendererFormat

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Graphics contexts

class UIGraphicsRenderer

An abstract base class for creating graphics renderers.

class UIGraphicsRendererContext

The base class for the drawing environments for graphics renderers.

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

