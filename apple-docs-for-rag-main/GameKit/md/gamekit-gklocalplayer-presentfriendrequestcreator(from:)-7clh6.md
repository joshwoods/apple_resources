

- GameKit
- GKLocalPlayer
-  presentFriendRequestCreator(from:) 

Instance Method

# presentFriendRequestCreator(from:)

Opens the Messages app with a sheet for the player to request friends.

macOS 12.0+

``` source
func presentFriendRequestCreator(from window: NSWindow?) throws
```

## Parameters 

`window`  

The window that’s the anchor for opening the Messages app.

## Discussion

If this method throws an exception, it doesn’t open the Messages app.

## See Also

### Adding Friends

var isPresentingFriendRequestViewController: Bool

A Boolean value that indicates whether your game presents the friends request view controller.

func presentFriendRequestCreator(from: UIViewController) throws

Presents a view controller with a Messages sheet for the player to request friends.

