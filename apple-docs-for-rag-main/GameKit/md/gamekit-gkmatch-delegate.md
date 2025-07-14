

- GameKit
- GKMatch
-  delegate 

Instance Property

# delegate

The delegate that handles communication between players in a match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
weak var delegate: (any GKMatchDelegate)? { get set }
```

## Discussion

To receive voice or data from other players, you must set the delegate.

## See Also

### Setting the delegate

protocol GKMatchDelegate

An object that receives connection status and data transmitted in a multiplayer game.

