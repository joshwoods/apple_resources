

- GameKit
- GKChallenge
-  receivingPlayer 

Instance Property

# receivingPlayer

The player who receives the challenge.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
@NSCopying
var receivingPlayer: GKPlayer? { get }
```

## See Also

### Examining Details about a Challenge

var issuingPlayer: GKPlayer?

The player who issues the challenge.

var message: String?

A text message that describes the challenge.

var state: GKChallengeState

The current state of the challenge.

enum GKChallengeState

The state of a challenge.

var issueDate: Date

The date the player issued the challenge.

var completionDate: Date?

The date the challenged player completed the challenge.

