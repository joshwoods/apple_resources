

- GameKit
- GKTurnBasedMatch
-  loadMatchData(completionHandler:) 

Instance Method

# loadMatchData(completionHandler:)

Fetches your game-specific data that you store in Game Center when ending a turn, saving a turn, or leaving a match.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func loadMatchData(completionHandler: ((Data?, (any Error)?) -> Void)? = nil)
```

``` source
func loadMatchData() async throws -> Data?
```

## Parameters 

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

*matchData*  
The match data you pass to `GKTurnBasedMatch` methods that GameKit stores in Game Center, or `nil` if an error occurs.

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Discussion

The matchData property is `nil` until you fetch the data from Game Center using this method.

## See Also

### Retrieving Match Details

var matchID: String

A unique identifier for the turn-based match.

var creationDate: Date

The date that Game Center created the match.

var participants: [GKTurnBasedParticipant]

The players that participate in a turn-based match.

var currentParticipant: GKTurnBasedParticipant?

The participant whose turn it is.

var status: GKTurnBasedMatch.Status

The state of the match, such as whether the match is open or has ended.

enum Status

The states of a match from when it’s created to when it ends.

var matchData: Data?

The game-specific data that you store in Game Center and pass between participants through a match object.

var matchDataMaximumSize: Int

The maximum size of the match data.

