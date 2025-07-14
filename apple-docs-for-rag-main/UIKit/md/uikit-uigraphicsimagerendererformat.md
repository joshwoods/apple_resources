

- UIKit
-  UIGraphicsImageRendererFormat 

Class

# UIGraphicsImageRendererFormat

A set of drawing attributes that represents the configuration of an image renderer context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class UIGraphicsImageRendererFormat
```

## Overview

Use an instance of UIGraphicsImageRendererFormat to initialize a UIGraphicsImageRenderer object with nondefault attributes.

The image renderer format object contains properties that determine the attributes of the underlying Core Graphics contexts that the image renderer creates. Use the default() class method to create an image renderer format instance optimized for the current device.

## Topics

### Creating the renderer

convenience init(for: UITraitCollection)

Creates the most suitable format for rendering on a device with the specified traits.

### Configuring the renderer attributes

var opaque: Bool

A Boolean value that indicates whether the underlying Core Graphics context has an alpha channel.

var scale: CGFloat

The display scale of the image renderer context.

var preferredRange: UIGraphicsImageRendererFormat.Range

The preferred color range of the image renderer context.

enum Range

Constants that specify the color range of the image renderer context.

var prefersExtendedRange: Bool

A Boolean value that specifies whether the bitmap context uses extended color.

Deprecated

### Instance Properties

var supportsHighDynamicRange: Bool

## Relationships

### Inherits From

- UIGraphicsRendererFormat

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

class UIGraphicsRendererFormat

A set of drawing attributes that represents the configuration of a graphics renderer context.

class UIGraphicsImageRenderer

A graphics renderer for creating Core Graphics-backed images.

class UIGraphicsImageRendererContext

The drawing environment for an image renderer.

class UIGraphicsPDFRenderer

A graphics renderer for creating PDFs.

class UIGraphicsPDFRendererContext

The drawing environment for a PDF renderer.

class UIGraphicsPDFRendererFormat

A set of drawing attributes that represents the configuration of a PDF renderer context.

