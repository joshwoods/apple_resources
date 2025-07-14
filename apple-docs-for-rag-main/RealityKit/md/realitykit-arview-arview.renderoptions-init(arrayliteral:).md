

- RealityKit
- ARView
- ARView.RenderOptions
-  init(arrayLiteral:) 

Initializer

# init(arrayLiteral:)

Creates a set containing the elements of the given array literal.

RealityKitSwiftiOSiPadOSMac Catalyst

``` source
init(arrayLiteral: Self.Element...)
```

Available when `ArrayLiteralElement` is `Self.Element`.

## Parameters 

`arrayLiteral`  

A list of elements of the new set.

## Discussion

Do not call this initializer directly. It is used by the compiler when you use an array literal. Instead, create a new set using an array literal as its value by enclosing a comma-separated list of values in square brackets. You can use an array literal anywhere a set is expected by the type context.

Here, a set of strings is created from an array literal holding only strings:

```
let ingredients: Set = ["cocoa beans", "sugar", "cocoa butter", "salt"]
if ingredients.isSuperset(of: ["sugar", "salt"]) {
    print("Whatever it is, it's bound to be delicious!")
}
// Prints "Whatever it is, it's bound to be delicious!"
```

## See Also

### Creating an option set

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

typealias Element

The element type of the option set.

typealias ArrayLiteralElement

The type of the elements of an array literal.

init(rawValue: UInt)

Creates a new option set from the given raw value.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

let rawValue: UInt

The corresponding value of the raw type.

