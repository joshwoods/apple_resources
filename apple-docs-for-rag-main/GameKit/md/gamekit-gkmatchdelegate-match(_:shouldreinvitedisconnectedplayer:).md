

- GameKit
- GKMatchDelegate
-  match(\_:shouldReinviteDisconnectedPlayer:) 

Instance Method

# match(\_:shouldReinviteDisconnectedPlayer:)

Determines whether the local player should reinvite another player who disconnected from a two-player match.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func match(
    _ match: GKMatch,
    shouldReinviteDisconnectedPlayer player: GKPlayer
) -> Bool
```

## Parameters 

`match`  

The match that the player disconnected from.

`player`  

The player who disconnected from the match.

## Return Value

true if GameKit should reinvite the player when they disconnect; false if GameKit should end the match when the player disconnects.

## Mentioned in 

Exchanging data between players in real-time games

## Discussion

If the player successfully reconnects to the match, GameKit sends match(_:player:didChange:) to the match’s delegate.

