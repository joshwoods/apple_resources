

- HomeKit
-  HMZone 

Class

# HMZone

A collection of rooms that users think of as a single area, like upstairs or downstairs.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMZone
```

## Overview

An HMZone instance is an optional grouping of rooms in a home, with names like “upstairs” and “downstairs”. Zones are optional—rooms don’t need to be in a zone. By adding rooms to a zone, the user can give commands to Siri like “Siri, turn on all of the lights downstairs.” A single room can be in multiple zones—for example, “kitchen” might be in both the “downstairs” and “entertainment area” zones.

You create new zones using the addZone(withName:completionHandler:) method of HMHome. A zone can’t span homes—that is, you can’t create a zone that includes rooms from more than one home.

## Topics

### Identifying a Zone

var name: String

The name of the zone.

func updateName(String, completionHandler: ((any Error)?) -> Void)

Updates the name of the zone.

var uniqueIdentifier: UUID

The unique identifier for a zone.

### Assigning Rooms to a Zone

var rooms: [HMRoom]

Array of rooms in the zone.

func addRoom(HMRoom, completionHandler: ((any Error)?) -> Void)

Adds a room to the zone.

func removeRoom(HMRoom, completionHandler: ((any Error)?) -> Void)

Removes a room from the zone.

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

### Grouping rooms into zones

var zones: [HMZone]

An array of all the zones in the home.

func addZone(withName: String, completionHandler: (HMZone?, (any Error)?) -> Void)

Adds a new zone to the home.

func removeZone(HMZone, completionHandler: ((any Error)?) -> Void)

Removes a zone from the home.

