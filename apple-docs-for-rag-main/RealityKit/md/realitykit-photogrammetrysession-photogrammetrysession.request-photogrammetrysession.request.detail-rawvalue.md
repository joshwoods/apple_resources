

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
- PhotogrammetrySession.Request.Detail
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var rawValue: Int { get }
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

### Using enumeration raw values

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

init?(rawValue: Int)

Creates a new instance with the specified raw value.

