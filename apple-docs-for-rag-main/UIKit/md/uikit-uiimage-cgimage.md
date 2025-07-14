

- UIKit
- UIImage
-  cgImage 

Instance Property

# cgImage

The underlying Quartz image data.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var cgImage: CGImage? { get }
```

## Discussion

If the image data has been purged because of memory constraints, invoking this method forces that data to be loaded back into memory. Reloading the image data may incur a performance penalty.

If the `UIImage` object was initialized using a `CIImage` object, the value of the property is `NULL`.

## See Also

### Getting the image data

var ciImage: CIImage?

The underlying Core Image data.

var images: [UIImage]?

The complete array of image objects that compose the animation of an animated object.

var imageAsset: UIImageAsset?

The image asset (if any) for the image.

