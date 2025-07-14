

- GameKit
- GKChallengeListener
-  player(\_:didComplete:issuedByFriend:) 

Instance Method

# player(\_:didComplete:issuedByFriend:)

Handles when the local player completes a challenge that a friend issues.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func player(
    _ player: GKPlayer,
    didComplete challenge: GKChallenge,
    issuedByFriend friendPlayer: GKPlayer
)
```

## Parameters 

`player`  

The player who completes the challenge.

`challenge`  

The challenge that the player completes.

`friendPlayer`  

The friend who issues the challenge.

## See Also

### Completing a Challenge

func player(GKPlayer, issuedChallengeWasCompleted: GKChallenge, byFriend: GKPlayer)

Handles when a friend completes a challenge that the local player issues.

