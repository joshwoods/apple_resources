

- AppKit
- NSProgressIndicator
-  startAnimation(\_:) 

Instance Method

# startAnimation(\_:)

Starts the animation of an indeterminate progress indicator.

macOS

``` source
@MainActor
func startAnimation(_ sender: Any?)
```

## Parameters 

`sender`  

The object sending the message.

## Discussion

Does nothing for a determinate progress indicator.

## See Also

### Related Documentation

Progress Indicator Programming Topics

### Animating the progress indicator

func stopAnimation(Any?)

Stops the animation of an indeterminate progress indicator.

var usesThreadedAnimation: Bool

A Boolean that indicates whether the progress indicator implements animation in a separate thread.

