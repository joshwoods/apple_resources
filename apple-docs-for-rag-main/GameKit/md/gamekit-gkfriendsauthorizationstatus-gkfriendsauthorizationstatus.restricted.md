

- GameKit
- GKFriendsAuthorizationStatus
-  GKFriendsAuthorizationStatus.restricted 

Case

# GKFriendsAuthorizationStatus.restricted

Access to the player’s list of friends restricted.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.3+

``` source
case restricted
```

## Mentioned in 

Connecting players with their friends in your game

## Discussion

While GameKit restricts access to a player’s friends’ data, the player can’t change the authorization status. If you previously loaded the player’s friends, delete the friends’ data from your game.

## See Also

### Authorization Statuses

case authorized

The player authorized your game to access their list of friends.

case denied

Access to the player’s friends’ data denied.

case notDetermined

The player hasn’t choosen whether your game may access their friends list.

