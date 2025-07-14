

- Game Controller
- GCController
-  controllerPausedHandler Deprecated

Instance Property

# controllerPausedHandler

The block that the framework calls when the user presses the pause button on the controller.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var controllerPausedHandler: ((GCController) -> Void)? { get set }
```

Deprecated

Instead use the Menu button found on the controller’s profile, if it exists.

## Discussion

Implement this handler to toggle between pausing and resuming gameplay. Provide an interface that displays when the user pauses the game, and allows the user to resume gameplay. If your game suspends gameplay for some other reason, also implement this handler to resume gameplay when it’s possible.

