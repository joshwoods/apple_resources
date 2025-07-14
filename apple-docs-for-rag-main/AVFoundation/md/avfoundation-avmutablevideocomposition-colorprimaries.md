

- AVFoundation
- AVMutableVideoComposition
-  colorPrimaries 

Instance Property

# colorPrimaries

The color primaries used for video composition.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var colorPrimaries: String? { get set }
```

## Mentioned in 

Tagging Media with Video Color Information

## Discussion

The default value is `nil`. When the value of this property is `nil`, the source’s color primaries are propagated and used. Valid values are those suitable for AVVideoColorPrimariesKey.

## See Also

### Configuring Color

var colorTransferFunction: String?

The transfer function used for video composition.

var colorYCbCrMatrix: String?

The YCbCr matrix used for video composition.

