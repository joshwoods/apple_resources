

- Screen Saver
- ScreenSaverView
-  isAnimating 

Instance Property

# isAnimating

A Boolean value that indicates whether the screen saver is animating.

macOS 10.0+

``` source
@MainActor
var isAnimating: Bool { get }
```

## Discussion

The value of this property is true when the screen saver is animating, and false when it isn’t.

## See Also

### Animating the screen saver

func startAnimation()

Activates the periodic timer that animates the screen saver.

func animateOneFrame()

Advances the screen saver’s animation by a single frame.

func stopAnimation()

Deactivates the timer that advances the animation.

