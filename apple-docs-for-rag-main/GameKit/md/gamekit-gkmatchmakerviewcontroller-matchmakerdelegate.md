

- GameKit
- GKMatchmakerViewController
-  matchmakerDelegate 

Instance Property

# matchmakerDelegate

The object that handles matchmaker view controller changes.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
weak var matchmakerDelegate: (any GKMatchmakerViewControllerDelegate)? { get set }
```

## Discussion

You must set the delegate for GameKit to notify you when players accept their invitations and you can start the game.

## See Also

### Setting the delegate

protocol GKMatchmakerViewControllerDelegate

An object that handles when the status of matchmaking changes.

