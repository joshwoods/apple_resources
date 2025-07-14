

- RealityKit
- ActionEventType
-  ActionEventType.RawValue 

Type Alias

# ActionEventType.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
typealias RawValue = UInt
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

## See Also

### Protocol support

init(rawValue: UInt)

Creates an action event type from a raw value.

let rawValue: UInt

The backing storage for action event types.

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

