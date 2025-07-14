

- GameKit
- GKLocalPlayer
-  loadFriends(\_:) 

Instance Method

# loadFriends(\_:)

Loads the local player’s friends list if the local player and their friends grant access.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.3+

``` source
func loadFriends(_ completionHandler: @escaping ([GKPlayer]?, (any Error)?) -> Void)
```

``` source
func loadFriends() async throws -> [GKPlayer]
```

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

`friends`  
The player’s friends who also grant your game access to their friends.

The local player and their friends authorization status must be GKFriendsAuthorizationStatus.authorized.

The local player and their friends must use a version of your game with the same bundle ID.

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Protecting the player’s privacy using scoped identifiers

Connecting players with their friends in your game

## Discussion

If the loadFriendsAuthorizationStatus(_:) method returns GKFriendsAuthorizationStatus.notDetermined, GameKit presents a prompt to the local player requesting access to their friends that may pause your game. GameKit displays the localized reason that you provide for the NSGKFriendListUsageDescription key in the information property list.

If you loaded friends who no longer appear in the `friends` parameter of the completion handler, remove the data for those friends from your game because they no longer grant your game access to that data.

## See Also

### Accessing Friends and Recents

func loadFriendsAuthorizationStatus((GKFriendsAuthorizationStatus, (any Error)?) -> Void)

Returns whether the player authorizes your game to access their friends list.

enum GKFriendsAuthorizationStatus

Constants that indicate if the local player grants access to their friends list.

func loadFriends(identifiedBy: [String], completionHandler: ([GKPlayer]?, (any Error)?) -> Void)

Loads the player’s friends list, scoped by the identifiers, if the player and their friends grant access.

NSGKFriendListUsageDescription

A message that tells the user why the app needs access to their Game Center friends list.

func loadChallengableFriends(completionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Loads players to whom the local player can issue a challenge.

func loadRecentPlayers(completionHandler: (([GKPlayer]?, (any Error)?) -> Void)?)

Loads players from the friends list or players that recently participated in a game with the local player.

