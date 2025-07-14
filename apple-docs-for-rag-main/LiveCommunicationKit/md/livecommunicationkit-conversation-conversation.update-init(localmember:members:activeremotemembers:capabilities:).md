

- LiveCommunicationKit
- Conversation
- Conversation.Update
-  init(localMember:members:activeRemoteMembers:capabilities:) 

Initializer

# init(localMember:members:activeRemoteMembers:capabilities:)

Creates a new `Update`. Note that `nil` value means “no change”.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
init(
    localMember: Handle? = nil,
    members: Set? = nil,
    activeRemoteMembers: Set? = nil,
    capabilities: Conversation.Capabilities? = nil
)
```

