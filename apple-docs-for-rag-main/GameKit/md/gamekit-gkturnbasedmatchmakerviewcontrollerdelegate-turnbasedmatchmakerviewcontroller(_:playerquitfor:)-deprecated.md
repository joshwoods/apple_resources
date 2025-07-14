

- GameKit
- GKTurnBasedMatchmakerViewControllerDelegate
-  turnBasedMatchmakerViewController(\_:playerQuitFor:) Deprecated

Instance Method

# turnBasedMatchmakerViewController(\_:playerQuitFor:)

Handles when a player quits the match.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.11DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func turnBasedMatchmakerViewController(
    _ viewController: GKTurnBasedMatchmakerViewController,
    playerQuitFor match: GKTurnBasedMatch
)
```

Deprecated

Use GKTurnBasedEventListener method player(_:wantsToQuitMatch:) instead.

## Parameters 

`viewController`  

The view controller with which the player interacts.

`match`  

The match that the player quits.

## Discussion

When GameKit invokes this method, the player forfeits the match without taking their turn. Implement this method to dismiss the view controller, set an outcome for the player, and then call the match’s participantQuitInTurn(with:nextParticipants:turnTimeout:match:completionHandler:) method.

## See Also

### Deprecated Methods

func turnBasedMatchmakerViewController(GKTurnBasedMatchmakerViewController, didFind: GKTurnBasedMatch)

Handles when the view controller finds participants for a turn-based match.

Deprecated

