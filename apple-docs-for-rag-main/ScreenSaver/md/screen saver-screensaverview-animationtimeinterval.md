

- Screen Saver
- ScreenSaverView
-  animationTimeInterval 

Instance Property

# animationTimeInterval

The time interval between animation frames.

macOS 10.0+

``` source
@MainActor
var animationTimeInterval: TimeInterval { get set }
```

## Discussion

If your screen saver has particular requirements for time between animation frames, call this method to set the animation rate to a reasonable value.

