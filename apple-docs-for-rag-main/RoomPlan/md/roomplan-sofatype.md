

- RoomPlan
-  SofaType 

Enumeration

# SofaType

Types of sofa the framework identifies in a captured room.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum SofaType
```

## Overview

When the framework observes a sofa in the physical environment during a scan, it chooses a type among these options that best matches the sofa’s look. The framework adds that instance of this enum to the attributes array for the object (see objects) that represents the sofa in the captured room.

## Topics

### Choosing a sofa type

case rectangular

A sofa shape that resembles a rectangle.

case singleSeat

A sofa that resembles a loveseat.

case lShaped

A sofa shape that resembles the letter L.

case lShapedExtension

The short side of the L-shape sofa.

case unidentified

An uncategorized sofa shape.

### Identifying a sofa type

var shortIdentifier: String

A human-readable identifier for the attribute.

### Categorizing a sofa type

static var parentCategory: CapturedElementCategory?

A category to which this room attribute belongs.

### Creating a sofa type

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

static var allCases: [SofaType]

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

