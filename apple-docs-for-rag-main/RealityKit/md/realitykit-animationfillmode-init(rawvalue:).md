

- RealityKit
- AnimationFillMode
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a fill mode from its backing data type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(rawValue: Int8)
```

## Parameters 

`rawValue`  

The backing data value for the fill mode.

## Discussion

Use this initializer to unarchive a fill mode from data:

```
let rawValue = unarchiveNextInt8(from: data) // Pseudo code.
let fillMode = AnimationFillMode(rawValue: rawValue)
```

## See Also

### Creating a fill mode

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

