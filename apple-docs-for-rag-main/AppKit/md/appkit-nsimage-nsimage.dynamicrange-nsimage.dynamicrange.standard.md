

- AppKit
- NSImage
- NSImage.DynamicRange
-  NSImage.DynamicRange.standard 

Case

# NSImage.DynamicRange.standard

Restricts the image content dynamic range to the standard range regardless of the actual range of the image content.

macOS 14.0+

``` source
case standard
```

## See Also

### Setting the dynamic range

case constrainedHigh

Allows for constrained High Dynamic Range (HDR) image content which is useful for mixing HDR and Standard Dynamic Range (SDR) content.

case high

Allows image content to use extended dynamic range if it has dynamic range content.

case unspecified

Indicates that the dynamic range treatment of the image is unknown or otherwise unspecified.

