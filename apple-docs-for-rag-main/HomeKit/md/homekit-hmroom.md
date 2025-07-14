

- HomeKit
-  HMRoom 

Class

# HMRoom

The smallest subdivision of a home’s space.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMRoom
```

## Overview

An HMRoom instance is a part of a home representing an individual room in the home. Rooms don’t have any physical characteristics like size or location. Instead, they’re names that are meaningful to the user, like “living room” or “kitchen”. Meaningful room names enable voice commands like “Siri, turn on the kitchen lights.”

You create new rooms using the addRoom(withName:completionHandler:) method of HMHome. You can also group rooms into zones using instances of HMZone. You can assign accessories to rooms, indicating the presence of that accessory in that room.

## Topics

### Identifying a room

var name: String

The name of the room.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the room.

var uniqueIdentifier: UUID

The unique identifier for a room.

### Finding accessories

var accessories: [HMAccessory]

The collection of accessories in the room.

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
- Sendable

## See Also

### Locating an accessory

var room: HMRoom?

The room containing the accessory.

