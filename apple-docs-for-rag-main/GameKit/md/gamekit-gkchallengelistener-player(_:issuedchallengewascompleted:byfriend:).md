

- GameKit
- GKChallengeListener
-  player(\_:issuedChallengeWasCompleted:byFriend:) 

Instance Method

# player(\_:issuedChallengeWasCompleted:byFriend:)

Handles when a friend completes a challenge that the local player issues.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func player(
    _ player: GKPlayer,
    issuedChallengeWasCompleted challenge: GKChallenge,
    byFriend friendPlayer: GKPlayer
)
```

## Parameters 

`player`  

The player who issues the challenge.

`challenge`  

The challenge that the friend completes.

`friendPlayer`  

The player who completes the challenge.

## See Also

### Completing a Challenge

func player(GKPlayer, didComplete: GKChallenge, issuedByFriend: GKPlayer)

Handles when the local player completes a challenge that a friend issues.

