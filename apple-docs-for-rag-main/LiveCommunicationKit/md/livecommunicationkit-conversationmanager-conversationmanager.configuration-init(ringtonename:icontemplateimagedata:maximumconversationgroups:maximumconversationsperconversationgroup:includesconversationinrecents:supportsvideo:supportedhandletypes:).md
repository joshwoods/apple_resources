

- LiveCommunicationKit
- ConversationManager
- ConversationManager.Configuration
-  init(ringtoneName:iconTemplateImageData:maximumConversationGroups:maximumConversationsPerConversationGroup:includesConversationInRecents:supportsVideo:supportedHandleTypes:) 

Initializer

# init(ringtoneName:iconTemplateImageData:maximumConversationGroups:maximumConversationsPerConversationGroup:includesConversationInRecents:supportsVideo:supportedHandleTypes:)

Creates a new `Configuration`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
init(
    ringtoneName: String?,
    iconTemplateImageData: Data?,
    maximumConversationGroups: Int,
    maximumConversationsPerConversationGroup: Int,
    includesConversationInRecents: Bool,
    supportsVideo: Bool,
    supportedHandleTypes: Set
)
```

## Parameters 

`ringtoneName`  

The name of the sound resource in the app bundle to be used for the provider ringtone.

`iconTemplateImageData`  

PNG data for the icon image to be displayed for the provider.

`maximumConversationGroups`  

The maximum number of `Conversation`s groups.

`maximumConversationsPerConversationGroup`  

The maximum number of `Conversation`s per `Conversation` group.

`includesConversationInRecents`  

A Boolean value that indicates whether the provider includes a call in the system’s Recents list after the call ends.

`supportsVideo`  

A Boolean value that indicates whether the provider supports video in addition to audio.

`supportedHandleTypes`  

The supported handle types.

