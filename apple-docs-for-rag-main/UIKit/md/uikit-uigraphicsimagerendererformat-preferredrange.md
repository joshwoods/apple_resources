

- UIKit
- UIGraphicsImageRendererFormat
-  preferredRange 

Instance Property

# preferredRange

The preferred color range of the image renderer context.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
var preferredRange: UIGraphicsImageRendererFormat.Range { get set }
```

## Discussion

This property affects the pixel format of the image that the renderer produces.

Different pixel formats can store different color ranges. The system chooses the precise pixel format, but you can set this property to exclude certain formats that support larger or narrower color ranges than you need.

## See Also

### Configuring the renderer attributes

var opaque: Bool

A Boolean value that indicates whether the underlying Core Graphics context has an alpha channel.

var scale: CGFloat

The display scale of the image renderer context.

enum Range

Constants that specify the color range of the image renderer context.

var prefersExtendedRange: Bool

A Boolean value that specifies whether the bitmap context uses extended color.

Deprecated

