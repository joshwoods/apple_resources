

- RoomPlan
- CapturedRoom
-  CapturedRoom.AttributesCodableRepresentation 

Structure

# CapturedRoom.AttributesCodableRepresentation

A serializable set of details that describe an object in the room.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
struct AttributesCodableRepresentation
```

## Overview

}

## Topics

### Creating an attributes codable representation

init(from: any Decoder) throws

Deserializes an attributes codable representation from the given decoder.

init(attributes: [any CapturedRoomAttribute])

Creates an attributes codable representation with the given collection of object attributes.

### Accessing room attributes

let attributes: [any CapturedRoomAttribute]

A collection of object attributes.

### Serializing an attributes codable representation

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

## Relationships

### Conforms To

- Decodable
- Encodable

## See Also

### Serializing a captured room

func encode(to: any Encoder) throws

Serializes a captured room to the specified encoder.

