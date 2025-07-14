

- RoomPlan
-  ChairLegType 

Enumeration

# ChairLegType

Types of chair legs the framework identifies in a captured room.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum ChairLegType
```

## Overview

When the framework observes a chair in the physical environment during a scan, it chooses a type among these options that best matches the look of the chair’s legs. The framework adds that instance of this enum to the attributes array for the object (see objects) that represents the chair in the captured room.

## Topics

### Choosing a chair leg type

case four

A type of chair that has four legs.

case star

A chair that rests on a bar that rises from a base, such as an office chair.

case unidentified

An uncategorized chair leg type.

### Identifying a chair leg type

var shortIdentifier: String

A human-readable identifier for the attribute.

### Categorizing a chair leg type

static var parentCategory: CapturedElementCategory?

A category to which this room attribute belongs.

### Creating a chair leg type

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

static var allCases: [ChairLegType]

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

## See Also

### Describing chairs

enum ChairType

Types of chair that the framework identifies in a captured room.

enum ChairArmType

Types of armchair the framework identifies in a captured room.

enum ChairBackType

Types of chair back the framework identifies in a captured room.

