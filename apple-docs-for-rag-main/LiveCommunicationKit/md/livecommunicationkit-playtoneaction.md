

- LiveCommunicationKit
-  PlayToneAction 

Class

# PlayToneAction

Plays a sequence of tones to indicate local or remote member keypad entry.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final class PlayToneAction
```

## Topics

### Initializers

init(conversationUUID: UUID, digits: String, tone: PlayToneAction.Tone)

Creates a new `PlayToneAction`.

### Instance Properties

let digits: String

The digits tapped by the user into the in-call keypad or included in the dial string.

let tone: PlayToneAction.Tone

The tone to play.

### Enumerations

enum Tone

The types of tones that may be played.

## Relationships

### Inherits From

- ConversationAction

