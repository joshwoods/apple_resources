

- GameKit
- GKTurnBasedMatch
-  load(withID:withCompletionHandler:) 

Type Method

# load(withID:withCompletionHandler:)

Loads a specific match with the specified identifier.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class func load(
    withID matchID: String,
    withCompletionHandler completionHandler: ((GKTurnBasedMatch?, (any Error)?) -> Void)? = nil
)
```

``` source
class func load(withID matchID: String) async throws -> GKTurnBasedMatch
```

## Parameters 

`matchID`  

The identifier for the turn-based match.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

*match*  
The local player’s match with the `matchID` identifier, or `nil` if an error occurs.

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Discussion

The matchData property of the match object is `nil` until you fetch the data from Game Center using the loadMatchData(completionHandler:) method.

## See Also

### Loading Existing Matches

class func loadMatches(completionHandler: (([GKTurnBasedMatch]?, (any Error)?) -> Void)?)

Fetches the turn-based matches from Game Center that the local player participates in.

