

- GameKit
- GKLocalPlayer
-  setDefaultLeaderboardIdentifier(\_:completionHandler:) 

Instance Method

# setDefaultLeaderboardIdentifier(\_:completionHandler:)

Sets the local player’s default leaderboard.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func setDefaultLeaderboardIdentifier(
    _ leaderboardIdentifier: String,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setDefaultLeaderboardIdentifier(_ leaderboardIdentifier: String) async throws
```

## Parameters 

`leaderboardIdentifier`  

The identifier of the leaderboard.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

error  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Encourage progress and competition with leaderboards

## Discussion

Until you change the default leaderboard for a player, it is the same as the default leaderboard for your game that you set in App Store Connect.

## See Also

### Working with Leaderboards

func loadDefaultLeaderboardIdentifier(completionHandler: ((String?, (any Error)?) -> Void)?)

Loads the identifier for the local player’s default leaderboard.

