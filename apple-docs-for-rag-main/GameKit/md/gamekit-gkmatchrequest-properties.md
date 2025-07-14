

- GameKit
- GKMatchRequest
-  properties 

Instance Property

# properties

The criteria for the local player that Game Center uses to find other players when using matchmaking rules.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+watchOS 10.2+

``` source
var properties: [String : Any]? { get set }
```

## Mentioned in 

Finding players with similar skill levels

Finding players using matchmaking rules

Letting players join matches using party codes

Assigning players to teams using rules

Creating matchmaking rules for backward compatibility

## Discussion

Matchmaking rules may use one or more of these properties to improve matchmaking results and reduce wait times. You set rules in App Store Connect to find players that best match these properties in a reasonable amount of time by loosening the criteria over time.

This property contains key-value pairs where keys are strings with game-specific meanings, such as the skill level, game mode, play style, and other preferences. The keys can be any string, except `gc`, which GameKit reserves. The values need to be types that the JSONSerialization class can convert to JSON data.

Set this property before you submit the match request to Game Center. For peer-to-peer matches, use the findMatch(for:withCompletionHandler:) method or present the GKMatchmakerViewController interface to submit a match request. For hosted matches, use the findMatchedPlayers(_:withCompletionHandler:) method to include other player properties in the result.

```
// Create a match request.
let request = GKMatchRequest()

// Set the matchmaking rules queue name.
request.queueName = "com.example.mygame.PartyCodeQueue"

// Set properties to the game-specific keys you use in the rules.
request.properties = [ "partyCode": partyCode ]
```

If the queueName property is `nil`, Game Center doesn’t use matchmaking rules and ignores the properties property.

For more information, see Matchmaking rules.

## See Also

### Matching players using rules

var queueName: String?

The name of the queue that Game Center places the match request in.

var recipientProperties: [GKPlayer : [String : Any]]?

The criteria for recipients of the match request that Game Center uses to find other players when using matchmaking rules.

