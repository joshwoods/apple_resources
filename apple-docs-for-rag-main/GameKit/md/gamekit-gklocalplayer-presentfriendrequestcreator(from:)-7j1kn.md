

- GameKit
- GKLocalPlayer
-  presentFriendRequestCreator(from:) 

Instance Method

# presentFriendRequestCreator(from:)

Presents a view controller with a Messages sheet for the player to request friends.

iOS 15.0+iPadOS 15.0+visionOS 1.0+

``` source
func presentFriendRequestCreator(from viewController: UIViewController) throws
```

## Parameters 

`viewController`  

The view controller that contains the Messages sheet, and that this method presents.

## Mentioned in 

Connecting players with their friends in your game

## Discussion

If this method throws an exception, it doesn’t present the view controller.

## See Also

### Adding Friends

var isPresentingFriendRequestViewController: Bool

A Boolean value that indicates whether your game presents the friends request view controller.

func presentFriendRequestCreator(from: NSWindow?) throws

Opens the Messages app with a sheet for the player to request friends.

