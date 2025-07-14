

- UIKit
- UIImage
-  size 

Instance Property

# size

The logical dimensions, in points, for the image.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var size: CGSize { get }
```

## Discussion

This value reflects the logical size of the image and takes the image’s current orientation into account. Multiply the size values by the value in the scale property to get the pixel dimensions of the image.

## See Also

### Getting the image size and scale

var scale: CGFloat

The scale factor of the image.

