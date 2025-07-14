

- RoomPlan
- CapturedRoom
- CapturedRoom.Section
-  CapturedRoom.Section.Label 

Enumeration

# CapturedRoom.Section.Label

Textual names for one part of a larger structure.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum Label
```

## Overview

The CapturedRoom.Section structure label property is of this type.

## Topics

### Creating a section label

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Assigning a section a label

case livingRoom

A distinct area that resembles a living room within a larger structure.

case kitchen

A distinct area that resembles a kitchen within a larger structure.

case diningRoom

A distinct area that resembles a dining room within a larger structure.

case bedroom

A distinct area that resembles a bedroom within a larger structure.

case bathroom

A distinct area that resembles a bathroom within a larger structure.

case unidentified

An uncategorized area within a larger structure.

### Instance Properties

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Describing a section

var label: CapturedRoom.Section.Label

A textual name for the section.

