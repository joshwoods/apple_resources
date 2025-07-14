

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
-  CapturedRoom.Surface.Category 

Enumeration

# CapturedRoom.Surface.Category

Classifications of a surface in a captured room.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum Category
```

## Overview

Each CapturedRoom.Surface instance in a captured room’s surface arrays (doors, openings, walls, and windows) reflects a classification (category) of this type.

## Topics

### Creating a surface category

init(from: any Decoder) throws

Creates a surface category by deserializing the specified decoder.

### Determining the surface category

case floor

A category for a surface that represents a floor.

case door(isOpen: Bool)

A category for a surface that represents a door.

case opening

A category for a surface that represents an opening.

case wall

A category for a surface that represents a wall.

case window

A category for a surface that represents a window.

### Serializing a surface category

func encode(to: any Encoder) throws

Serializes a surface category to the specified encoder.

### Comparing surface categories

static func == (CapturedRoom.Surface.Category, CapturedRoom.Surface.Category) -> Bool

Determines whether two surface categories are equal.

static func != (Self, Self) -> Bool

Determines whether two surface categories aren’t equal.

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Identifying a surface

var identifier: UUID

A unique alphanumeric value that the framework assigns the surface.

var parentIdentifier: UUID?

A unique alphanumeric value that identifies a surface’s parent surface.

var category: CapturedRoom.Surface.Category

A classification that the captured room assigns the surface.

var confidence: CapturedRoom.Confidence

A level of certainty in the surface’s category.

