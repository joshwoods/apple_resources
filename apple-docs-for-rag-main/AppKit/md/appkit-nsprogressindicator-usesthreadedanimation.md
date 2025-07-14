

- AppKit
- NSProgressIndicator
-  usesThreadedAnimation 

Instance Property

# usesThreadedAnimation

A Boolean that indicates whether the progress indicator implements animation in a separate thread.

macOS

``` source
@MainActor
var usesThreadedAnimation: Bool { get set }
```

## Discussion

When the value of this property is true, animation of the progress indicator occurs in a separate thread.

If the app becomes multithreaded as a result of an invocation of this method, the app’s performance could become noticeably slower.

## See Also

### Animating the progress indicator

func startAnimation(Any?)

Starts the animation of an indeterminate progress indicator.

func stopAnimation(Any?)

Stops the animation of an indeterminate progress indicator.

