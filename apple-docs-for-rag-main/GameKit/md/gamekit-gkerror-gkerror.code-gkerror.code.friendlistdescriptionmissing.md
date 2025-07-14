

- GameKit
- GKError
- GKError.Code
-  GKError.Code.friendListDescriptionMissing 

Case

# GKError.Code.friendListDescriptionMissing

Access to the local player’s list of friends denied for lack of a reason.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
case friendListDescriptionMissing
```

## Discussion

If your game wants access to the player’s friends, provide a reason by adding the NSGKFriendListUsageDescription key to the information property list.

## See Also

### Friend List Errors

case friendListRestricted

Access to the local player’s list of friends restricted.

case friendListDenied

Access to the local player’s list of friends denied.

case friendRequestNotAvailable

The player can’t send a friend request at this time from this device.

