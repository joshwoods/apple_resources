

- UIKit
- UIImageView
-  animationDuration 

Instance Property

# animationDuration

The amount of time it takes to go through one cycle of the images.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var animationDuration: TimeInterval { get set }
```

## Discussion

The time duration is measured in seconds. The default value of this property is `0.0`, which causes the image view to use a duration equal to the number of images multiplied by 1/30th of a second. Thus, if you had 30 images, the duration would be 1 second.

## See Also

### Animating a sequence of images

var animationImages: [UIImage]?

An array of UIImage objects to use for an animation.

var highlightedAnimationImages: [UIImage]?

An array of UIImage objects to use for an animation when the view is highlighted.

var animationRepeatCount: Int

Specifies the number of times to repeat the animation.

func startAnimating()

Starts animating the images in the receiver.

func stopAnimating()

Stops animating the images in the receiver.

var isAnimating: Bool

Returns a Boolean value indicating whether the animation is running.

