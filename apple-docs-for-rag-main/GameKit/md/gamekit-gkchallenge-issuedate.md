

- GameKit
- GKChallenge
-  issueDate 

Instance Property

# issueDate

The date the player issued the challenge.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
var issueDate: Date { get }
```

## See Also

### Examining Details about a Challenge

var issuingPlayer: GKPlayer?

The player who issues the challenge.

var receivingPlayer: GKPlayer?

The player who receives the challenge.

var message: String?

A text message that describes the challenge.

var state: GKChallengeState

The current state of the challenge.

enum GKChallengeState

The state of a challenge.

var completionDate: Date?

The date the challenged player completed the challenge.

