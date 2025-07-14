

- UIKit
- UIGraphicsImageRendererFormat
-  scale 

Instance Property

# scale

The display scale of the image renderer context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var scale: CGFloat { get set }
```

## Discussion

The display scale determines the number of pixels per point.

The default value is equal to the scale of the main screen.

## See Also

### Configuring the renderer attributes

var opaque: Bool

A Boolean value that indicates whether the underlying Core Graphics context has an alpha channel.

var preferredRange: UIGraphicsImageRendererFormat.Range

The preferred color range of the image renderer context.

enum Range

Constants that specify the color range of the image renderer context.

var prefersExtendedRange: Bool

A Boolean value that specifies whether the bitmap context uses extended color.

Deprecated

