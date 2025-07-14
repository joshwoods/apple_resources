

- UIKit
- UIGraphicsImageRendererFormat
-  opaque 

Instance Property

# opaque

A Boolean value that indicates whether the underlying Core Graphics context has an alpha channel.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var opaque: Bool { get set }
```

## Discussion

Setting the value of this property to false specifies that the underlying Core Graphics context has an alpha channel, whereas true indicates it does not. The default value is false.

A Core Graphics context requires an alpha channel to express transparency. Without an alpha channel a Core Graphics context is said to be opaque, i.e. without transparency.

## See Also

### Configuring the renderer attributes

var scale: CGFloat

The display scale of the image renderer context.

var preferredRange: UIGraphicsImageRendererFormat.Range

The preferred color range of the image renderer context.

enum Range

Constants that specify the color range of the image renderer context.

var prefersExtendedRange: Bool

A Boolean value that specifies whether the bitmap context uses extended color.

Deprecated

