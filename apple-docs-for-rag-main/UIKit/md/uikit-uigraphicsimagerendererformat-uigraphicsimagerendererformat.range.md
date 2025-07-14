

- UIKit
- UIGraphicsImageRendererFormat
-  UIGraphicsImageRendererFormat.Range 

Enumeration

# UIGraphicsImageRendererFormat.Range

Constants that specify the color range of the image renderer context.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
enum Range
```

## Topics

### Constants

case automatic

The system automatically chooses the image renderer context’s pixel format according to the color range of its content.

case extended

The image renderer context supports wide color.

case standard

The image renderer context doesn’t support extended colors.

case unspecified

The image renderer context doesn’t specify a color range.

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

### Configuring the renderer attributes

var opaque: Bool

A Boolean value that indicates whether the underlying Core Graphics context has an alpha channel.

var scale: CGFloat

The display scale of the image renderer context.

var preferredRange: UIGraphicsImageRendererFormat.Range

The preferred color range of the image renderer context.

var prefersExtendedRange: Bool

A Boolean value that specifies whether the bitmap context uses extended color.

Deprecated

