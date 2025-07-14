

- GameKit
- GKTurnBasedMatchmakerViewControllerDelegate
-  turnBasedMatchmakerViewController(\_:didFind:) Deprecated

Instance Method

# turnBasedMatchmakerViewController(\_:didFind:)

Handles when the view controller finds participants for a turn-based match.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.11DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func turnBasedMatchmakerViewController(
    _ viewController: GKTurnBasedMatchmakerViewController,
    didFind match: GKTurnBasedMatch
)
```

Deprecated

Use GKTurnBasedEventListener method player(_:receivedTurnEventFor:didBecomeActive:) instead.

## Parameters 

`viewController`  

The view controller that finds participants for the match.

`match`  

The match that the participants join.

## Discussion

When the participants accept their invitations to join a turn-based match, GameKit invokes this method in the game instances for all participants in the match, including the local player who initiates the match. Implement this method to dismiss the view controller and start gameplay that allows the local player to take their turn. Use the match object to show information about the other participants in the match.

## See Also

### Deprecated Methods

func turnBasedMatchmakerViewController(GKTurnBasedMatchmakerViewController, playerQuitFor: GKTurnBasedMatch)

Handles when a player quits the match.

Deprecated

