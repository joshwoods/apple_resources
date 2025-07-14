

- GameKit
- GKPlayer
-  displayName 

Instance Property

# displayName

A string to display for the player.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var displayName: String { get }
```

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

The display name for a player depends on whether the player is a friend of the local player on the device. If the player is a friend of the local player, the display name is the actual name of the player. If the player isn’t a friend, the display name is the player’s alias.

## See Also

### Accessing player details

var alias: String

A string the player chooses to identify themself to other players.

var isInvitable: Bool

A Boolean value that indicates whether the local player can send an invitation to the player.

var isFriend: Bool

A Boolean value that indicates whether the player is a friend of the local player.

Deprecated

