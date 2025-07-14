

- GameKit
- GKInvite
-  playerAttributes 

Instance Property

# playerAttributes

The player attributes for the match.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var playerAttributes: UInt32 { get }
```

## Discussion

The value of this property matches the playerAttributes property of the match request that the other player uses to create the match.

## See Also

### Getting Properties

var sender: GKPlayer

The player who sends the invitation.

var playerGroup: Int

The player group for the match.

var isHosted: Bool

A Boolean value that indicates whether you host the game on your own servers.

var inviter: String

The identifier for the player who sends the invitation.

Deprecated

