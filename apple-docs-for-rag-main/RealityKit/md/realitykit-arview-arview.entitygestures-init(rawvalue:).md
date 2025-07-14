

- RealityKit
- ARView
- ARView.EntityGestures
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a new option set from the given raw value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
init(rawValue: Int)
```

## Parameters 

`rawValue`  

The raw value of the option set to create. Each bit of `rawValue` potentially represents an element of the option set, though raw values may include bits that are not defined as distinct values of the `OptionSet` type.

## Discussion

This initializer always succeeds, even if the value passed as `rawValue` exceeds the static properties declared as part of the option set. This example creates an instance of `ShippingOptions` with a raw value beyond the highest element, with a bit mask that effectively contains all the declared static members.

```
let extraOptions = ShippingOptions(rawValue: 255)
print(extraOptions.isStrictSuperset(of: .all))
// Prints "true"
```

## See Also

### Creating gesture option sets

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

typealias Element

The element type of the option set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

let rawValue: Int

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

