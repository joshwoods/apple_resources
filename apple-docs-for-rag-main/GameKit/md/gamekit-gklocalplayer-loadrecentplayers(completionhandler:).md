

- GameKit
- GKLocalPlayer
-  loadRecentPlayers(completionHandler:) 

Instance Method

# loadRecentPlayers(completionHandler:)

Loads players from the friends list or players that recently participated in a game with the local player.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.11+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func loadRecentPlayers(completionHandler: (([GKPlayer]?, (any Error)?) -> Void)? = nil)
```

``` source
func loadRecentPlayers() async throws -> [GKPlayer]
```

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

`recentPlayers`  
Players from the friends list or players that recently participated in a game with the local player.

`error`  
Describes an error if it occurs, or `nil` if `t`he operation completes. Possible errors include network and authentication issues.

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

func loadChallengableFriends(completionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Loads players to whom the local player can issue a challenge.

