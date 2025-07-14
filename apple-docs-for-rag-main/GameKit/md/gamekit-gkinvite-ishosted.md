

- GameKit
- GKInvite
-  isHosted 

Instance Property

# isHosted

A Boolean value that indicates whether you host the game on your own servers.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
var isHosted: Bool { get }
```

## Discussion

If the value of this property is true, you host the game on your own servers. If the value is false, Game Center hosts the peer-to-peer match on its servers. The default value is false.

## See Also

### Getting Properties

var sender: GKPlayer

The player who sends the invitation.

var playerAttributes: UInt32

The player attributes for the match.

var playerGroup: Int

The player group for the match.

var inviter: String

The identifier for the player who sends the invitation.

Deprecated

