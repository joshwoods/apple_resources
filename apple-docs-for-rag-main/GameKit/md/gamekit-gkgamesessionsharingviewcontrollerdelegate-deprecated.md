

- GameKit
-  GKGameSessionSharingViewControllerDelegate Deprecated

Protocol

# GKGameSessionSharingViewControllerDelegate

A protocol you implement to respond to changes to a sharing user interface.

tvOS 10.0–12.0Deprecated

``` source
protocol GKGameSessionSharingViewControllerDelegate : NSObjectProtocol
```

Deprecated

For real-time matches, use GKMatchmakerViewControllerDelegate to receive notifications from the GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewControllerDelegate and GKLocalPlayerListener to receive notifications from the GKTurnBasedMatchmakerViewController.

## Topics

### Dismissing a Sharing View Controller

func sharingViewController(GKGameSessionSharingViewController, didFinishWithError: (any Error)?)

Indicates the sharing view controller is ready to be dismissed.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Accessing Share View Controller Properties

var delegate: (any GKGameSessionSharingViewControllerDelegate)?

The delegate for the sharing view controller.

Deprecated

var session: GKGameSession

The game session associated with the view controller.

Deprecated

