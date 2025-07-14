

- RoomPlan
-  StorageType 

Enumeration

# StorageType

Types of storage area that the framework identifies in a captured room.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum StorageType
```

## Overview

When the framework observes a storage area in the physical environment, it chooses a type among these options that best matches the type of storage. The framework adds that instance of this enum to the attributes array for the object (see objects) in the captured room that represents the storage in the captured room.

## Topics

### Choosing a storage area type

case cabinet

An enclosed storage area.

case shelf

An open, wall-located storage area.

### Identifying a storage area type

var shortIdentifier: String

A human-readable identifier for the attribute.

### Categorizing a storage area type

static var parentCategory: CapturedElementCategory?

A category to which this room attribute belongs.

### Creating a storage area type

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static var allCases: [StorageType]

A collection of all values of this type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- CapturedRoomAttribute
- CaseIterable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

