

- UIKit
- UIImage
-  baselineOffsetFromBottom 

Instance Property

# baselineOffsetFromBottom

The position of the baseline relative to the bottom of the image.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 13.0+visionOSwatchOS 6.0+

``` source
var baselineOffsetFromBottom: CGFloat? { get }
```

## Discussion

Positive values place the baseline up inside the image, and negative values place the baseline below the bottom of the image. When the value of this property is `0.0`, the baseline position is equal to the bottom of the image.

