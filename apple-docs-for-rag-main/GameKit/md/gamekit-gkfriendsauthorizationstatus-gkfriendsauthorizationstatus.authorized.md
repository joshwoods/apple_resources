

- GameKit
- GKFriendsAuthorizationStatus
-  GKFriendsAuthorizationStatus.authorized 

Case

# GKFriendsAuthorizationStatus.authorized

The player authorized your game to access their list of friends.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.3+

``` source
case authorized
```

## Mentioned in 

Connecting players with their friends in your game

## Discussion

If the loadFriendsAuthorizationStatus(_:) method returns `GKFriendsAuthorizationStatus.authorized`, the loadFriends(identifiedBy:completionHandler:) method passes the friends list to the completion handler.

## See Also

### Authorization Statuses

case denied

Access to the player’s friends’ data denied.

case notDetermined

The player hasn’t choosen whether your game may access their friends list.

case restricted

Access to the player’s list of friends restricted.

