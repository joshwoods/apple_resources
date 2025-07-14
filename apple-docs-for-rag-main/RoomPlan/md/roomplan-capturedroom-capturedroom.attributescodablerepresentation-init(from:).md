

- RoomPlan
- CapturedRoom
- CapturedRoom.AttributesCodableRepresentation
-  init(from:) 

Initializer

# init(from:)

Deserializes an attributes codable representation from the given decoder.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
init(from decoder: any Decoder) throws
```

## Parameters 

`decoder`  

An object to deserialize.

## See Also

### Creating an attributes codable representation

init(attributes: [any CapturedRoomAttribute])

Creates an attributes codable representation with the given collection of object attributes.

