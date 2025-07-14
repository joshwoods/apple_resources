

- GameKit
-  GKFriendsAuthorizationStatus 

Enumeration

# GKFriendsAuthorizationStatus

Constants that indicate if the local player grants access to their friends list.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.3+

``` source
enum GKFriendsAuthorizationStatus
```

## Topics

### Authorization Statuses

case authorized

The player authorized your game to access their list of friends.

case denied

Access to the player’s friends’ data denied.

case notDetermined

The player hasn’t choosen whether your game may access their friends list.

case restricted

Access to the player’s list of friends restricted.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing Friends and Recents

func loadFriendsAuthorizationStatus((GKFriendsAuthorizationStatus, (any Error)?) -> Void)

Returns whether the player authorizes your game to access their friends list.

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

