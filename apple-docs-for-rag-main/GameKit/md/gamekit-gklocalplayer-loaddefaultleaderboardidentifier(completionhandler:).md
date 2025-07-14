

- GameKit
- GKLocalPlayer
-  loadDefaultLeaderboardIdentifier(completionHandler:) 

Instance Method

# loadDefaultLeaderboardIdentifier(completionHandler:)

Loads the identifier for the local player’s default leaderboard.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func loadDefaultLeaderboardIdentifier(completionHandler: ((String?, (any Error)?) -> Void)? = nil)
```

``` source
func loadDefaultLeaderboardIdentifier() async throws -> String
```

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

categoryID  
The leaderboard ID for the local player’s default leaderboard that you set in App Store Connect.

error  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Encourage progress and competition with leaderboards

## See Also

### Working with Leaderboards

func setDefaultLeaderboardIdentifier(String, completionHandler: (((any Error)?) -> Void)?)

Sets the local player’s default leaderboard.

