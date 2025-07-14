

- HomeKit
- HMPresenceEvent
-  init(presenceEventType:presenceUserType:) 

Initializer

# init(presenceEventType:presenceUserType:)

Creates a new presence event with the specified event and user presence types.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    presenceEventType: HMPresenceEventType,
    presenceUserType: HMPresenceEventUserType
)
```

## Parameters 

`presenceEventType`  

The event type that determines when the event fires.

`presenceUserType`  

The user type whose presence triggers the event.

## Return Value

An initialized presence event.

