

- Screen Saver
- ScreenSaverView
-  startAnimation() 

Instance Method

# startAnimation()

Activates the periodic timer that animates the screen saver.

macOS 10.0+

``` source
@MainActor
func startAnimation()
```

## Discussion

The system calls this method when it’s time for you to start animating your screen saver’s content. The system calls this method only once at the start of animations. Use this method to set up any initial state information you require or to allocate expensive resources. If you override this method, you must call the inherited implementation at some point.

## See Also

### Animating the screen saver

func animateOneFrame()

Advances the screen saver’s animation by a single frame.

func stopAnimation()

Deactivates the timer that advances the animation.

var isAnimating: Bool

A Boolean value that indicates whether the screen saver is animating.

