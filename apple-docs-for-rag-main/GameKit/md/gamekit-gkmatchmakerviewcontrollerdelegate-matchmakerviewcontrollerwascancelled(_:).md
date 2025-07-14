

- GameKit
- GKMatchmakerViewControllerDelegate
-  matchmakerViewControllerWasCancelled(\_:) 

Instance Method

# matchmakerViewControllerWasCancelled(\_:)

Handles when a player cancels a request to find players for a match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func matchmakerViewControllerWasCancelled(_ viewController: GKMatchmakerViewController)
```

**Required**

## Parameters 

`viewController`  

The view controller that the player cancels.

## Mentioned in 

Finding multiple players for a game

## Discussion

This method needs to dismiss the view controller.

## See Also

### Handling cancellations and errors

func matchmakerViewController(GKMatchmakerViewController, didFailWithError: any Error)

Handles when a view controller encounters an error while finding players for a match.

**Required**

