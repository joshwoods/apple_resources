

- GameKit
- GKTurnBasedMatchmakerViewControllerDelegate
-  turnBasedMatchmakerViewController(\_:didFailWithError:) 

Instance Method

# turnBasedMatchmakerViewController(\_:didFailWithError:)

Handles when an error occurs while the local player invites other players.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func turnBasedMatchmakerViewController(
    _ viewController: GKTurnBasedMatchmakerViewController,
    didFailWithError error: any Error
)
```

**Required**

## Parameters 

`viewController`  

The view controller that encounters an error.

`error`  

The error that occurs.

## Discussion

This method needs to dismiss the view controller.

## See Also

### Handling Cancellation and Errors

func turnBasedMatchmakerViewControllerWasCancelled(GKTurnBasedMatchmakerViewController)

Handles when the player dismisses the view controller without inviting players.

**Required**

