

- GameKit
- GKAchievement
-  init(identifier:forPlayer:) Deprecated

Initializer

# init(identifier:forPlayer:)

Initializes an achievement for a specific player.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
init?(
    identifier: String?,
    forPlayer playerID: String
)
```

## Parameters 

`identifier`  

A string that matches the identifier string for an achievement you created for your game in App Store Connect.

`playerID`  

The identifier for the player associated with the specified achievement.

## Discussion

Your game initializes a new achievement object for a specific player only when it has not previously reported progress for that achievement. Use this method to submit a participant’s achievement when ending a turn-based match.

