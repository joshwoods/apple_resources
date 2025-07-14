

- UIKit
- UIImageView
-  stopAnimating() 

Instance Method

# stopAnimating()

Stops animating the images in the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func stopAnimating()
```

## See Also

### Animating a sequence of images

var animationImages: [UIImage]?

An array of UIImage objects to use for an animation.

var highlightedAnimationImages: [UIImage]?

An array of UIImage objects to use for an animation when the view is highlighted.

var animationDuration: TimeInterval

The amount of time it takes to go through one cycle of the images.

var animationRepeatCount: Int

Specifies the number of times to repeat the animation.

func startAnimating()

Starts animating the images in the receiver.

var isAnimating: Bool

Returns a Boolean value indicating whether the animation is running.

