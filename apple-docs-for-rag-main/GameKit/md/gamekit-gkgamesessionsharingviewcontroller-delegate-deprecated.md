

- GameKit
- GKGameSessionSharingViewController
-  delegate Deprecated

Instance Property

# delegate

The delegate for the sharing view controller.

tvOS 10.0–12.0Deprecated

``` source
@MainActor
weak var delegate: (any GKGameSessionSharingViewControllerDelegate)? { get set }
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## See Also

### Accessing Share View Controller Properties

protocol GKGameSessionSharingViewControllerDelegate

A protocol you implement to respond to changes to a sharing user interface.

Deprecated

var session: GKGameSession

The game session associated with the view controller.

Deprecated

