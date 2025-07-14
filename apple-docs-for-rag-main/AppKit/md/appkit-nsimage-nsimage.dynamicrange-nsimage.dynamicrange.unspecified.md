

- AppKit
- NSImage
- NSImage.DynamicRange
-  NSImage.DynamicRange.unspecified 

Case

# NSImage.DynamicRange.unspecified

Indicates that the dynamic range treatment of the image is unknown or otherwise unspecified.

macOS 14.0+

``` source
case unspecified
```

## Discussion

The imageDynamicRange property can return this type when the system can’t determine the High Dynamic Range (HDR) of the image. Otherwise, the use of this value isn’t encouraged and results in undefined behavior.

## See Also

### Setting the dynamic range

case standard

Restricts the image content dynamic range to the standard range regardless of the actual range of the image content.

case constrainedHigh

Allows for constrained High Dynamic Range (HDR) image content which is useful for mixing HDR and Standard Dynamic Range (SDR) content.

case high

Allows image content to use extended dynamic range if it has dynamic range content.

