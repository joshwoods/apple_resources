

- RealityKit
- ARView
- ARView.EntityGestures
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
let rawValue: Int
```

## Discussion

A new instance initialized with `rawValue` will be equivalent to this instance. For example:

```
enum PaperSize: String {
    case A4, A5, Letter, Legal
}

let selectedSize = PaperSize.Letter
print(selectedSize.rawValue)
// Prints "Letter"

print(selectedSize == PaperSize(rawValue: selectedSize.rawValue)!)
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

init(rawValue: Int)

Creates a new option set from the given raw value.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

