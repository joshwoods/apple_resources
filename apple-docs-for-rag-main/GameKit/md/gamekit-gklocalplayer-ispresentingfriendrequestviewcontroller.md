

- GameKit
- GKLocalPlayer
-  isPresentingFriendRequestViewController 

Instance Property

# isPresentingFriendRequestViewController

A Boolean value that indicates whether your game presents the friends request view controller.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
var isPresentingFriendRequestViewController: Bool { get }
```

## Discussion

true if the friends request view controller appears; otherwise, false.

## See Also

### Adding Friends

func presentFriendRequestCreator(from: UIViewController) throws

Presents a view controller with a Messages sheet for the player to request friends.

func presentFriendRequestCreator(from: NSWindow?) throws

Opens the Messages app with a sheet for the player to request friends.

