

- LiveCommunicationKit
-  ConversationManager 

Class

# ConversationManager

A programmatic interface for interacting with and observing conversations.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final class ConversationManager
```

## Topics

### Structures

struct Configuration

An encapsulation of the configuration of a `ConversationManager`.

### Initializers

convenience init(configuration: ConversationManager.Configuration)

Creates a new `ConversationManager` with the given `ConversationManager.Configuration`.

### Instance Properties

let configuration: ConversationManager.Configuration

The configuration of the manager.

var conversations: [Conversation]

var delegate: (any ConversationManagerDelegate)?

var pendingActions: [ConversationAction]

`ConversationAction`s that have not yet been fulfilled.

### Instance Methods

func invalidate()

Invalidates the manager, ends all `Conversation`s, and fails all pending `ConversationAction`s.

func pendingConversationActions(of: ConversationAction.Type, for: Conversation) -> [ConversationAction]

Returns all pending `ConversationAction`s of the specified class for the specified call identifier that are incomplete.

func perform([ConversationAction]) async throws

Instructs the `ConversationManager` to asynchronously perform the given actions.

func reportConversationEvent(Conversation.Event, for: Conversation)

Informs the system that some event has occurred and to update the given `Conversation` as needed.

func reportNewIncomingConversation(uuid: UUID, update: Conversation.Update) async throws

Informs the system that there’s a new incoming Conversation, and the device should begin to ring and present the incoming Conversation UI.

### Type Methods

class func reportNewIncomingVoIPPushPayload([AnyHashable : Any]) async throws

Reports a new incoming call after your notification service extension decrypts a VoIP call request.

## Relationships

### Conforms To

- Copyable
- Observable

