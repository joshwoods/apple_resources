

- GameKit
- GKMatchRequest
-  queueName 

Instance Property

# queueName

The name of the queue that Game Center places the match request in.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+watchOS 10.2+

``` source
var queueName: String? { get set }
```

## Mentioned in 

Finding players using matchmaking rules

Finding players with similar skill levels

Assigning players to teams using rules

Finding multiple players for a game

Troubleshooting matchmaking rules using metrics

## Discussion

To use matchmaking rules, set the queueName property to a queue name that you configure in App Store Connect. Then set properties and optionally recipientProperties to game-specific criteria.

A *queue name* is a uniform type identifier (UTI) that contains only alphanumeric characters (A-Z, a-z, 0-9), hyphens (-), or periods (.). The string should be in reverse-DNS format. Queue names are case sensitive.

Matchmaking rules evaluate the properties of match requests in the same queue to find the best match according to the rules that you set in App Store Connect for the queue. An error occurs if the queue doesn’t exist.

If this property is `nil`, Game Center doesn’t use matchmaking rules to find other players.

For more information, see Matchmaking rules.

## See Also

### Related Documentation

Create a queue

Create a queue and add it to a rule set.

### Matching players using rules

var properties: [String : Any]?

The criteria for the local player that Game Center uses to find other players when using matchmaking rules.

var recipientProperties: [GKPlayer : [String : Any]]?

The criteria for recipients of the match request that Game Center uses to find other players when using matchmaking rules.

