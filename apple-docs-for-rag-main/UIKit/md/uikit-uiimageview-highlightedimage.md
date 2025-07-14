

- UIKit
- UIImageView
-  highlightedImage 

Instance Property

# highlightedImage

The highlighted image displayed in the image view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var highlightedImage: UIImage? { get set }
```

## Discussion

The image in this property is displayed when the image view’s isHighlighted property is true. If the highlightedAnimationImages property contains a valid set of images, those image are used instead.

This property is set to the image (if any) you specified at initialization time. If you did not use the init(image:highlightedImage:) method to initialize your image view, the initial value of this property is `nil`.

## See Also

### Related Documentation

var highlightedAnimationImages: [UIImage]?

An array of UIImage objects to use for an animation when the view is highlighted.

### Accessing the displayed images

var image: UIImage?

The image displayed in the image view.

