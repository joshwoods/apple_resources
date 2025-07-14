

- RoomPlan
-  TableType 

Enumeration

# TableType

Types of table the framework identifies in a captured room.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum TableType
```

## Overview

When the framework observes a table in the physical environment during a scan, it chooses a type among these options that best matches the table’s look. The framework adds that instance of this enum to the attributes array for the object (see objects) that represents the table in the captured room.

## Topics

### Choosing a chair type

case dining

A table top for the purpose of dining.

case coffee

A table top that resembles a coffee table.

case unidentified

An uncategorized table top.

### Identifying a chair type

var shortIdentifier: String

A human-readable identifier for the attribute.

### Categorizing a chair type

static var parentCategory: CapturedElementCategory?

A category to which this room attribute belongs.

### Creating a chair type

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

static var allCases: [TableType]

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

### Describing tables

enum TableShapeType

Different table shapes that the framework identifies in a captured room.

