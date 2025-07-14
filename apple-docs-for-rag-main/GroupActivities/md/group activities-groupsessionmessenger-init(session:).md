

- Group Activities
- GroupSessionMessenger
-  init(session:) 

Initializer

# init(session:)

Creates a new group session messenger with GroupSessionMessenger.DeliveryMode.reliable delivery mode and associates it with the specified session object.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
init(session: GroupSession) where Activity : GroupActivity
```

## Parameters 

`session`  

The group session to use for communication with participants. Specify a session object that is in either the GroupSession.State.waiting or GroupSession.State.joined state for this parameter. However, a session must be in the joined state to send or receive messages.

