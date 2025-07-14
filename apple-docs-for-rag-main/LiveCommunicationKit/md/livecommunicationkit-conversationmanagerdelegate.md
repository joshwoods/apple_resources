

- LiveCommunicationKit
-  ConversationManagerDelegate 

Protocol

# ConversationManagerDelegate

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
protocol ConversationManagerDelegate : AnyObject
```

## Topics

### Instance Methods

func conversationManager(ConversationManager, conversationChanged: Conversation)

Invoked when a `Conversation` is changed.

**Required**

func conversationManager(ConversationManager, didActivate: AVAudioSession)

Called when the provider’s audio session is activated.

**Required**

func conversationManager(ConversationManager, didDeactivate: AVAudioSession)

Called when the provider’s audio session is deactivated.

**Required**

func conversationManager(ConversationManager, perform: ConversationAction)

Called when the system requires that some `ConversationAction` is performed.

**Required**

func conversationManager(ConversationManager, timedOutPerforming: ConversationAction)

Called when a `ConversationAction` is not performed before it expires.

**Required**

func conversationManagerDidBegin(ConversationManager)

Called when the provider begins.

**Required**

func conversationManagerDidReset(ConversationManager)

Called when the provider resets.

**Required**

