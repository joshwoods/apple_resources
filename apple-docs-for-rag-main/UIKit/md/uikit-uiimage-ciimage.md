

- UIKit
- UIImage
-  ciImage 

Instance Property

# ciImage

The underlying Core Image data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var ciImage: CIImage? { get }
```

## Discussion

If the `UIImage` object was initialized using a CGImage, the value of the property is `nil`.

## See Also

### Getting the image data

var cgImage: CGImage?

The underlying Quartz image data.

var images: [UIImage]?

The complete array of image objects that compose the animation of an animated object.

var imageAsset: UIImageAsset?

The image asset (if any) for the image.

