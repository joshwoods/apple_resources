

- GameKit
- GKTurnBasedMatchmakerViewControllerDelegate
-  turnBasedMatchmakerViewControllerWasCancelled(\_:) 

Instance Method

# turnBasedMatchmakerViewControllerWasCancelled(\_:)

Handles when the player dismisses the view controller without inviting players.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func turnBasedMatchmakerViewControllerWasCancelled(_ viewController: GKTurnBasedMatchmakerViewController)
```

**Required**

## Parameters 

`viewController`  

The view controller that the player dismisses.

## Discussion

This method needs to dismiss the view controller.

## See Also

### Handling Cancellation and Errors

func turnBasedMatchmakerViewController(GKTurnBasedMatchmakerViewController, didFailWithError: any Error)

Handles when an error occurs while the local player invites other players.

**Required**

