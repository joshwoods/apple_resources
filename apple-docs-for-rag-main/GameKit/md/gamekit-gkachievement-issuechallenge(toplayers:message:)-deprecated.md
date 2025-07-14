

- GameKit
- GKAchievement
-  issueChallenge(toPlayers:message:) Deprecated

Instance Method

# issueChallenge(toPlayers:message:)

Issues an achievement challenge to a list of players.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func issueChallenge(
    toPlayers playerIDs: [String]?,
    message: String?
)
```

## Parameters 

`playerIDs`  

The identifiers for the players to challenge. Because Game Center limits the number of players in a challenge request to 10, the maximum size of this array is 10.

`message`  

A text message to display to the challenged players.

## Discussion

Set up your game to issue a challenge request only in direct response to a player action.

If you mark the achievement as hidden, or if the challenged player already earned the achievement and you don’t mark the achievement as replayable in App Store Connect, the local player can’t issue the challenge.

## See Also

### Deprecated Methods

func report(completionHandler: (((any Error)?) -> Void)?)

Reports the player’s progress to Game Center.

Deprecated

func selectChallengeablePlayerIDs([String]?, withCompletionHandler: (([String]?, (any Error)?) -> Void)?)

Finds the subset of players who can earn an achievement.

Deprecated

