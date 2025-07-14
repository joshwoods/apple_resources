

- RoomPlan
- CapturedRoom
- CapturedRoom.Section
- CapturedRoom.Section.Label
-  init(from:) 

Initializer

# init(from:)

Creates a new instance by decoding from the given decoder, when the type’s `RawValue` is `String`.

RoomPlanSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
init(from decoder: any Decoder) throws
```

Available when `Self` conforms to `Decodable` and `RawValue` is `String`.

## Parameters 

`decoder`  

The decoder to read data from.

## Discussion

This initializer throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

