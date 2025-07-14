

- AVKit
- AVPlayerView
-  delegate 

Instance Property

# delegate

The player view’s delegate object.

macOS 12.0+

``` source
@MainActor
weak var delegate: (any AVPlayerViewDelegate)? { get set }
```

## See Also

### Setting the Delegate Object

protocol AVPlayerViewDelegate

A protocol that defines the methods to implement to participate in the player view’s full-screen presentation life cycle.

