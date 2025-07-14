

- GameKit
- GKChallengeListener
-  player(\_:wantsToPlay:) 

Instance Method

# player(\_:wantsToPlay:)

Handles when the local player issues a challenge and the other player accepts.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func player(
    _ player: GKPlayer,
    wantsToPlay challenge: GKChallenge
)
```

## Parameters 

`player`  

The player who accepts the challenge.

`challenge`  

The challenge that the player issues to another player.

## See Also

### Responding to a Challenge

func player(GKPlayer, didReceive: GKChallenge)

Handles when the local player issues a challenge but the other player doesn’t want to respond immediately.

