

- RoomPlan
-  CapturedElementCategory 

Enumeration

# CapturedElementCategory

The category of the particular object or surface.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
enum CapturedElementCategory
```

## Overview

A CapturedRoomAttribute adopter’s parentCategory property is of this type.

## Topics

### Determining the category type

case object(CapturedRoom.Object.Category)

A category that’s scoped to the captured object.

case surface(CapturedRoom.Surface.Category)

A category that’s scoped to the captured surface.

### Creating a category

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Operators

static func == (CapturedElementCategory, CapturedElementCategory) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Sendable

## See Also

### Accessing object details

protocol CapturedRoomAttribute

Details about an object in the room that the framework observes during a scan.

