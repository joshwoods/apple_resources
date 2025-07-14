

- GameKit
- GKFriendRequestComposeViewControllerDelegate
-  friendRequestComposeViewControllerDidFinish(\_:) Deprecated

Instance Method

# friendRequestComposeViewControllerDidFinish(\_:)

Called when the player dismisses the request.

iOS 4.2–10.0DeprecatediPadOS 4.2–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.12DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func friendRequestComposeViewControllerDidFinish(_ viewController: GKFriendRequestComposeViewController)
```

**Required**

Deprecated

No longer supported.

## Parameters 

`viewController`  

The friend request view controller that was dismissed by the player.

## Discussion

Your delegate should dismiss the view controller. If your game paused any gameplay or other activities, it can restart those services in this method.

