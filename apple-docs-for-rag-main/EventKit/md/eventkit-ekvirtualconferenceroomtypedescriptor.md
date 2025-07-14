

- EventKit
-  EKVirtualConferenceRoomTypeDescriptor 

Class

# EKVirtualConferenceRoomTypeDescriptor

Details about a room where virtual conferences take place.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
class EKVirtualConferenceRoomTypeDescriptor
```

## Overview

To present a list of rooms where a virtual conference takes place, your virtual conference provider creates one or more room type descriptors. Each descriptor contains a user-visible title and an identifier of your choosing. When users create events using one of the rooms you provide, EventKit calls fetchVirtualConference(identifier:completionHandler:) and passes the room’s identifier.

## Topics

### Creating Room Type Descriptors

init(title: String, identifier: EKVirtualConferenceRoomTypeIdentifier)

Creates an object that describes a location where a virtual conference takes place.

### Configuring Room Type Descriptors

var title: String

The user-visible name of a room where virtual conferences take place, such as Personal Room or Team Room.

var identifier: EKVirtualConferenceRoomTypeIdentifier

A unique string you choose that identifies the room.

typealias EKVirtualConferenceRoomTypeIdentifier

The type for a room type identifier.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Virtual conferences

class EKVirtualConferenceProvider

An object that associates virtual conferencing details with an event object in a user’s calendar.

class EKVirtualConferenceDescriptor

Details about a virtual conference that uses a custom room type.

