

- LiveCommunicationKit
-  ConversationAction 

Class

# ConversationAction

A programmatic interface for objects that represent a VoIP action associated with a `Conversation`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
class ConversationAction
```

## Topics

### Initializers

convenience init(conversationUUID: UUID, timeoutDate: Date)

Initializes a new conversation action.

### Instance Properties

var conversationUUID: UUID

The unique identifier for the `Conversation` associated with the action.

var state: ConversationAction.State

The action’s current state.

var timeoutDate: Date

The `Date` after which the action cannot be completed.

var uuid: UUID

The unique identifier for the action.

### Instance Methods

func fail()

Reports the failed execution of the action.

func fulfill()

Reports the successful execution of the action.

### Enumerations

enum State

Represents the current state of a `ConversationAction`.

## Relationships

### Inherited By

- EndConversationAction
- JoinConversationAction
- MergeConversationAction
- MuteConversationAction
- PauseConversationAction
- PlayToneAction
- StartConversationAction
- UnmergeConversationAction

