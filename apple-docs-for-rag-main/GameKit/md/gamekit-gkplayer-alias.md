

- GameKit
- GKPlayer
-  alias 

Instance Property

# alias

A string the player chooses to identify themself to other players.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var alias: String { get }
```

## Discussion

GameKit uses the player’s alias when a player isn’t a friend of the local player. Typically, you never display the alias string directly in your user interface. Instead use the displayName property.

## See Also

### Accessing player details

var displayName: String

A string to display for the player.

var isInvitable: Bool

A Boolean value that indicates whether the local player can send an invitation to the player.

var isFriend: Bool

A Boolean value that indicates whether the player is a friend of the local player.

Deprecated

