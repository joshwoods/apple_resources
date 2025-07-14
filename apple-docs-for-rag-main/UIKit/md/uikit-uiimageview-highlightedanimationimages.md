

- UIKit
- UIImageView
-  highlightedAnimationImages 

Instance Property

# highlightedAnimationImages

An array of UIImage objects to use for an animation when the view is highlighted.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var highlightedAnimationImages: [UIImage]? { get set }
```

## Discussion

The array must contain UIImage objects. You may use the same image object more than once in the array. Setting this property to a value other than `nil` hides the image represented by the highlightedImage property. The value of this property is `nil` by default.

## See Also

### Related Documentation

var highlightedImage: UIImage?

The highlighted image displayed in the image view.

### Animating a sequence of images

var animationImages: [UIImage]?

An array of UIImage objects to use for an animation.

var animationDuration: TimeInterval

The amount of time it takes to go through one cycle of the images.

var animationRepeatCount: Int

Specifies the number of times to repeat the animation.

func startAnimating()

Starts animating the images in the receiver.

func stopAnimating()

Stops animating the images in the receiver.

var isAnimating: Bool

Returns a Boolean value indicating whether the animation is running.

