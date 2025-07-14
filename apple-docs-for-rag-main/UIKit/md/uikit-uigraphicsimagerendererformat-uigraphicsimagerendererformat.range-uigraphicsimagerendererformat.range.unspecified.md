

- UIKit
- UIGraphicsImageRendererFormat
- UIGraphicsImageRendererFormat.Range
-  UIGraphicsImageRendererFormat.Range.unspecified 

Case

# UIGraphicsImageRendererFormat.Range.unspecified

The image renderer context doesn’t specify a color range.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
case unspecified
```

## Discussion

In general, avoid specifying this value for an image renderer format. Some color spaces that you access using the imageRendererFormat property of UIImage may use this value.

## See Also

### Constants

case automatic

The system automatically chooses the image renderer context’s pixel format according to the color range of its content.

case extended

The image renderer context supports wide color.

case standard

The image renderer context doesn’t support extended colors.

