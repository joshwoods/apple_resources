

- Create ML
- MLStyleTransfer
- MLStyleTransfer.ModelParameters
- MLStyleTransfer.ModelParameters.ModelAlgorithmType
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
var rawValue: String { get }
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

### Working with raw values

init?(rawValue: String)

Creates a new instance with the specified raw value.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

