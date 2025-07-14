

- UIKit
- UIGraphicsImageRendererFormat
- UIGraphicsImageRendererFormat.Range
-  UIGraphicsImageRendererFormat.Range.standard 

Case

# UIGraphicsImageRendererFormat.Range.standard

The image renderer context doesn’t support extended colors.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
case standard
```

## Discussion

If you draw wide-color content into an image renderer context that uses the standard color range, you may lose color information. The system matches the colors to the standard range of their corresponding color space.

## See Also

### Constants

case automatic

The system automatically chooses the image renderer context’s pixel format according to the color range of its content.

case extended

The image renderer context supports wide color.

case unspecified

The image renderer context doesn’t specify a color range.

