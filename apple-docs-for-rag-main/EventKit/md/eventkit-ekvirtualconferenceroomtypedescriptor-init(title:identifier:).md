

- EventKit
- EKVirtualConferenceRoomTypeDescriptor
-  init(title:identifier:) 

Initializer

# init(title:identifier:)

Creates an object that describes a location where a virtual conference takes place.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    title: String,
    identifier: EKVirtualConferenceRoomTypeIdentifier
)
```

## Parameters 

`title`  

The user-visible name of a room where virtual conferences take place, such as Personal Room or Team Room.

`identifier`  

A unique string you choose that identifies the room.

## Return Value

An object that describes a location where a virtual conference takes place.

