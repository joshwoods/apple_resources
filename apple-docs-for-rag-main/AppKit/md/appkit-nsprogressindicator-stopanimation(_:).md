

- AppKit
- NSProgressIndicator
-  stopAnimation(\_:) 

Instance Method

# stopAnimation(\_:)

Stops the animation of an indeterminate progress indicator.

macOS

``` source
@MainActor
func stopAnimation(_ sender: Any?)
```

## Parameters 

`sender`  

The object sending the message.

## Discussion

Does nothing for a determinate progress indicator.

## See Also

### Animating the progress indicator

func startAnimation(Any?)

Starts the animation of an indeterminate progress indicator.

var usesThreadedAnimation: Bool

A Boolean that indicates whether the progress indicator implements animation in a separate thread.

