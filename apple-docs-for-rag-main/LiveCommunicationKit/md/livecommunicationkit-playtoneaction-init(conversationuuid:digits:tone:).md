

- LiveCommunicationKit
- PlayToneAction
-  init(conversationUUID:digits:tone:) 

Initializer

# init(conversationUUID:digits:tone:)

Creates a new `PlayToneAction`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
init(
    conversationUUID: UUID,
    digits: String,
    tone: PlayToneAction.Tone
)
```

## Parameters 

`conversationUUID`  

The unique identfiier of the `Conversation` to which this action will be applied.

`digits`  

The digits tapped by the user into the in-call keypad or included in the dial string.

`tone`  

The tone to play.

