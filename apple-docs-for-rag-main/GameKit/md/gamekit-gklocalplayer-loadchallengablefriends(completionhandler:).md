

- GameKit
- GKLocalPlayer
-  loadChallengableFriends(completionHandler:) 

Instance Method

# loadChallengableFriends(completionHandler:)

Loads players to whom the local player can issue a challenge.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func loadChallengableFriends(completionHandler: (([GKPlayer]?, (any Error)?) -> Void)? = nil)
```

``` source
func loadChallengableFriends() async throws -> [GKPlayer]
```

## Parameters 

`completionHandler`  

A block that GameKit calls when this method loads players the local player can challenge.

The block receives the following parameters:

`challengableFriends`  
Players to whom the local player can issue a challenge. The local player can issue a challenge to a player with a friend level of FL1 or FL2.

`error`  
Describes an error if it occurs, or `nil` if the operation completes. Possible errors include networking issues or an unauthenticated player.

## See Also

### Accessing Friends and Recents

func loadFriendsAuthorizationStatus((GKFriendsAuthorizationStatus, (any Error)?) -> Void)

Returns whether the player authorizes your game to access their friends list.

enum GKFriendsAuthorizationStatus

Constants that indicate if the local player grants access to their friends list.

func loadFriends(([GKPlayer]?, (any Error)?) -> Void)

Loads the local player’s friends list if the local player and their friends grant access.

func loadFriends(identifiedBy: [String], completionHandler: ([GKPlayer]?, (any Error)?) -> Void)

Loads the player’s friends list, scoped by the identifiers, if the player and their friends grant access.

NSGKFriendListUsageDescription

A message that tells the user why the app needs access to their Game Center friends list.

func loadRecentPlayers(completionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Loads players from the friends list or players that recently participated in a game with the local player.

