

- LiveCommunicationKit
- ConversationManager
-  ConversationManager.Configuration 

Structure

# ConversationManager.Configuration

An encapsulation of the configuration of a `ConversationManager`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct Configuration
```

## Topics

### Initializers

init(ringtoneName: String?, iconTemplateImageData: Data?, maximumConversationGroups: Int, maximumConversationsPerConversationGroup: Int, includesConversationInRecents: Bool, supportsVideo: Bool, supportedHandleTypes: Set&lt;Handle.Kind>)

Creates a new `Configuration`.

### Instance Properties

var iconTemplateImageData: Data?

PNG data for the icon image to be displayed for the provider.

var includesConversationInRecents: Bool

A Boolean value that indicates whether the provider includes a call in the system’s Recents list after the call ends.

var maximumConversationGroups: Int

The maximum number of `Conversation`s groups.

var maximumConversationsPerConversationGroup: Int

The maximum number of `Conversation`s per `Conversation` group.

var ringtoneName: String?

The name of the sound resource in the app bundle to be used for the provider ringtone.

var supportedHandleTypes: Set&lt;Handle.Kind>

The supported handle types.

var supportsVideo: Bool

A Boolean value that indicates whether the provider supports video in addition to audio.

