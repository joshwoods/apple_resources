

- RealityKit
- ActionEventType
-  ActionEventType.Element 

Type Alias

# ActionEventType.Element

The element type of the option set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
typealias Element = ActionEventType
```

## Discussion

To inherit all the default implementations from the `OptionSet` protocol, the `Element` type must be `Self`, the default.

## See Also

### Protocol support

init(rawValue: UInt)

Creates an action event type from a raw value.

let rawValue: UInt

The backing storage for action event types.

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

