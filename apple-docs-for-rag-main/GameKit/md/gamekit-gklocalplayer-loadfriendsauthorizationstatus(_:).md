

- GameKit
- GKLocalPlayer
-  loadFriendsAuthorizationStatus(\_:) 

Instance Method

# loadFriendsAuthorizationStatus(\_:)

Returns whether the player authorizes your game to access their friends list.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.3+

``` source
func loadFriendsAuthorizationStatus(_ completionHandler: @escaping (GKFriendsAuthorizationStatus, (any Error)?) -> Void)
```

``` source
func loadFriendsAuthorizationStatus() async throws -> GKFriendsAuthorizationStatus
```

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

`authorizationStatus`  
A status that indicates if the player authorized or denied your game access to their friends list.

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

An error occurs if you don’t add the NSGKFriendListUsageDescription key to the information property list file.

## Mentioned in 

Connecting players with their friends in your game

## See Also

### Accessing Friends and Recents

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

func loadRecentPlayers(completionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Loads players from the friends list or players that recently participated in a game with the local player.

