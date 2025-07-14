

- Group Activities
- GroupSessionMessenger
-  init(session:deliveryMode:) 

Initializer

# init(session:deliveryMode:)

Creates a new group session messenger with the specified delivery mode, GroupSessionMessenger.DeliveryMode, and associates it with the specified session object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    session: GroupSession,
    deliveryMode: GroupSessionMessenger.DeliveryMode
) where Activity : GroupActivity
```

## Parameters 

`session`  

The group session to use for communication with participants. Specify a session object that is in either the GroupSession.State.waiting or GroupSession.State.joined state for this parameter. However, a session must be in the joined state to send or receive messages.

`deliveryMode`  

The delivery mode for sending and receiving messages. Specify a delivery mode option for the underlying transport of either GroupSessionMessenger.DeliveryMode.reliable or GroupSessionMessenger.DeliveryMode.unreliable

