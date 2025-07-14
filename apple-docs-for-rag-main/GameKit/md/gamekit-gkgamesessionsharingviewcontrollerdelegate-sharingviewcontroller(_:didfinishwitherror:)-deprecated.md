

- GameKit
- GKGameSessionSharingViewControllerDelegate
-  sharingViewController(\_:didFinishWithError:) Deprecated

Instance Method

# sharingViewController(\_:didFinishWithError:)

Indicates the sharing view controller is ready to be dismissed.

tvOS 10.0–12.0Deprecated

``` source
func sharingViewController(
    _ viewController: GKGameSessionSharingViewController,
    didFinishWithError error: (any Error)?
)
```

**Required**

Deprecated

For real-time matches, use GKMatchmakerViewControllerDelegate to receive notifications from the GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewControllerDelegate and GKLocalPlayerListener to receive notifications from the GKTurnBasedMatchmakerViewController.

## Parameters 

`viewController`  

The sharing view controller to be dismissed.

`error`  

An optional GameKit error. This parameter is `nil` if the sharing view controller is successfully dismissed.

