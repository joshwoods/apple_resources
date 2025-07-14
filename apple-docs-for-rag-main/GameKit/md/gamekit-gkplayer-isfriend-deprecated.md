

- GameKit
- GKPlayer
-  isFriend Deprecated

Instance Property

# isFriend

A Boolean value that indicates whether the player is a friend of the local player.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var isFriend: Bool { get }
```

Deprecated

Use loadFriendPlayers(completionHandler:) instead.

## Discussion

Players use the Game Center app to declare other players as friends.

## See Also

### Accessing player details

var alias: String

A string the player chooses to identify themself to other players.

var displayName: String

A string to display for the player.

var isInvitable: Bool

A Boolean value that indicates whether the local player can send an invitation to the player.

