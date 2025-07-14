

- UIKit
- UIImageView
-  image 

Instance Property

# image

The image displayed in the image view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var image: UIImage? { get set }
```

## Discussion

This property contains the main image displayed by the image view. This image is displayed when the image view is in its natural state. When highlighted, the image view displays the image in its highlightedImage property instead. If that property is set to `nil`, the image view applies a default highlight to this image. If the animationImages property contains a valid set of images, those images are used instead.

Changing the image in this property does not automatically change the size of the image view. After setting the image, call the sizeToFit() method to recompute the image view’s size based on the new image and the active constraints.

This property is set to the image you specified at initialization time. If you did not use the init(image:) or init(image:highlightedImage:) method to initialize your image view, the initial value of this property is `nil`.

## See Also

### Related Documentation

var animationImages: [UIImage]?

An array of UIImage objects to use for an animation.

### Accessing the displayed images

var highlightedImage: UIImage?

The highlighted image displayed in the image view.

