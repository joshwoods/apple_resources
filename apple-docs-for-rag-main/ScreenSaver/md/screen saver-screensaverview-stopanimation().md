

- Screen Saver
- ScreenSaverView
-  stopAnimation() 

Instance Method

# stopAnimation()

Deactivates the timer that advances the animation.

macOS 10.0+

``` source
@MainActor
func stopAnimation()
```

## Discussion

The system calls this method when it’s time for you to stop animating your screen saver’s content. The system calls this method only once at the end of animations. Use this method to unload expensive resources or to reset your screen saver to a known state. If you override this method, you must call the inherited implementation at some point.

## See Also

### Animating the screen saver

func startAnimation()

Activates the periodic timer that animates the screen saver.

func animateOneFrame()

Advances the screen saver’s animation by a single frame.

var isAnimating: Bool

A Boolean value that indicates whether the screen saver is animating.

