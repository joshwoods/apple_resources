

- GameKit
- GKTurnBasedMatchmakerViewController
-  turnBasedMatchmakerDelegate 

Instance Property

# turnBasedMatchmakerDelegate

The object that handles turn-based matchmaker view controller changes.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
weak var turnBasedMatchmakerDelegate: (any GKTurnBasedMatchmakerViewControllerDelegate)? { get set }
```

## Discussion

You must set the delegate for GameKit to notify you when players cancel matchmaking or an error occurs.

## See Also

### Setting the Delegate

protocol GKTurnBasedMatchmakerViewControllerDelegate

A protocol that handles when the status of turn-based matchmaking changes.

