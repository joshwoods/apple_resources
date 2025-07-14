

- RoomPlan
-  CapturedRoomAttribute 

Protocol

# CapturedRoomAttribute

Details about an object in the room that the framework observes during a scan.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
protocol CapturedRoomAttribute : CaseIterable, RawRepresentable, Sendable where Self.RawValue == String
```

## Overview

If the framework identifies details about an CapturedRoom.Object during a scan, it adds an adopter of this protocol that represents that detail to the object’s attributes array. For example, details the framework recognizes as a stool with a star-shaped base contains both of the ChairType.stool and ChairLegType.star options in the `attributes` array for the object that represents the physical stool.

## Topics

### Identifying an attribute

var shortIdentifier: String

A human-readable identifier for the attribute.

**Required**

### Determining an attribute’s category

static var parentCategory: CapturedElementCategory?

A category to which this room attribute belongs.

**Required**

## Relationships

### Inherits From

- CaseIterable
- RawRepresentable
- Sendable

### Conforming Types

- ChairArmType
- ChairBackType
- ChairLegType
- ChairType
- SofaType
- StorageType
- TableShapeType
- TableType

## See Also

### Accessing object details

enum CapturedElementCategory

The category of the particular object or surface.

