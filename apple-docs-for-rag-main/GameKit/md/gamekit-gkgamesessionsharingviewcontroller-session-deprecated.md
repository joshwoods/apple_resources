

- GameKit
- GKGameSessionSharingViewController
-  session Deprecated

Instance Property

# session

The game session associated with the view controller.

tvOS 10.0–12.0Deprecated

``` source
@MainActor
var session: GKGameSession { get }
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## See Also

### Accessing Share View Controller Properties

var delegate: (any GKGameSessionSharingViewControllerDelegate)?

The delegate for the sharing view controller.

Deprecated

protocol GKGameSessionSharingViewControllerDelegate

A protocol you implement to respond to changes to a sharing user interface.

Deprecated

