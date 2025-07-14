

- AVFoundation
- AVMutableVideoComposition
-  colorTransferFunction 

Instance Property

# colorTransferFunction

The transfer function used for video composition.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var colorTransferFunction: String? { get set }
```

## Mentioned in 

Tagging Media with Video Color Information

## Discussion

The default value is `nil`. When the value of this property is `nil`, the source’s transfer function is propagated and used. Valid values are those suitable for AVVideoTransferFunctionKey.

## See Also

### Configuring Color

var colorPrimaries: String?

The color primaries used for video composition.

var colorYCbCrMatrix: String?

The YCbCr matrix used for video composition.

