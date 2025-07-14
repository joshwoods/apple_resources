

- RoomPlan
- CapturedRoom
- CapturedRoom.Section
- CapturedRoom.Section.Label
-  CapturedRoom.Section.Label.RawValue 

Type Alias

# CapturedRoom.Section.Label.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
typealias RawValue = String
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

