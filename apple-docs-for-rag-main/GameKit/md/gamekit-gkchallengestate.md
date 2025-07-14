

- GameKit
-  GKChallengeState 

Enumeration

# GKChallengeState

The state of a challenge.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum GKChallengeState
```

## Topics

### Challenge States

case invalid

The challenge isn’t valid because an error occurred.

case pending

The player issued a challenge, but the other player hasn’t accepted or refused it.

case completed

The player successfully completed the challenge.

case declined

The player declined the challenge.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var issueDate: Date

The date the player issued the challenge.

var completionDate: Date?

The date the challenged player completed the challenge.

