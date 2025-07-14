

- UIKit
- UIImage
-  scale 

Instance Property

# scale

The scale factor of the image.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var scale: CGFloat { get }
```

## Discussion

If you load an image from a file whose name includes the `@2x` modifier, the scale is set to `2.0`. You can also specify an explicit scale factor when initializing an image from a Core Graphics image. All other images are assumed to have a scale factor of `1.0`.

If you multiply the logical size of the image (stored in the size property) by the value in this property, you get the dimensions of the image in pixels.

## See Also

### Getting the image size and scale

var size: CGSize

The logical dimensions, in points, for the image.

