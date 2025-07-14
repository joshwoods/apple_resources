

- GameKit
- GKTurnBasedEventHandler
-  delegate Deprecated

Instance Property

# delegate

The delegate for the event handler.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
weak var delegate: (any GKTurnBasedEventHandlerDelegate & NSObjectProtocol)? { get set }
```

## Discussion

If your game implements turn-based matches, it should set the delegate immediately after the local player is successfully authenticated. You want to set the delegate immediately because your game may have been launched specifically to handle a turn-based match event.

