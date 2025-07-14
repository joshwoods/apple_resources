

- UIKit
- UIImage
-  UIImage.RenderingMode 

Enumeration

# UIImage.RenderingMode

Constants that specify the possible rendering modes for an image.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum RenderingMode
```

## Overview

The rendering mode controls how UIKit uses color information to display an image. See Providing images for different appearances for creating tintable images with template mode.

## Topics

### Rendering modes

case automatic

Draw the image using the context’s default rendering mode.

case alwaysOriginal

Always draw the original image, without treating it as a template.

case alwaysTemplate

Always draw the image as a template image, ignoring its color information.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting rendering information

var renderingMode: UIImage.RenderingMode

A setting that determines how the app renders an image.

var imageRendererFormat: UIGraphicsImageRendererFormat

The preferred image renderer format for the image.

