

- UIKit
- UIImage
-  imageAsset 

Instance Property

# imageAsset

The image asset (if any) for the image.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var imageAsset: UIImageAsset? { get }
```

## Discussion

For images loaded from an image assets, this property contains an image asset object that you can use to fetch the other variants of the image. If you did not create the image object using an image asset, the value of this property is `nil`. This property is always `nil` for images created using a ciImage object.

## See Also

### Getting the image data

var cgImage: CGImage?

The underlying Quartz image data.

var ciImage: CIImage?

The underlying Core Image data.

var images: [UIImage]?

The complete array of image objects that compose the animation of an animated object.

