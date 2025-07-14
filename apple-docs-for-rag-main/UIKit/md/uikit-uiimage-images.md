

- UIKit
- UIImage
-  images 

Instance Property

# images

The complete array of image objects that compose the animation of an animated object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var images: [UIImage]? { get }
```

## Discussion

For a non-animated image, the value of this property is `nil`.

## See Also

### Getting the image data

var cgImage: CGImage?

The underlying Quartz image data.

var ciImage: CIImage?

The underlying Core Image data.

var imageAsset: UIImageAsset?

The image asset (if any) for the image.

