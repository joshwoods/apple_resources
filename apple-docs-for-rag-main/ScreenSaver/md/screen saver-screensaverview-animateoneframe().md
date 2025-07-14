

- Screen Saver
- ScreenSaverView
-  animateOneFrame() 

Instance Method

# animateOneFrame()

Advances the screen saver’s animation by a single frame.

macOS 10.0+

``` source
@MainActor
func animateOneFrame()
```

## Discussion

The system calls this method each time the timer animating the screen saver fires. The time between calls to this method is always at least animationTimeInterval. The system locks focus on your view before it calls this method, so you can use this method to draw content. You can also let draw(_:) perform the drawing, in which case you use this method to call setNeedsDisplay(_:) to mark your view as dirty. The default implementation of this method does nothing.

## See Also

### Animating the screen saver

func startAnimation()

Activates the periodic timer that animates the screen saver.

func stopAnimation()

Deactivates the timer that advances the animation.

var isAnimating: Bool

A Boolean value that indicates whether the screen saver is animating.

