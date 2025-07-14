

- Swift
- RawRepresentable
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var rawValue: Self.RawValue { get }
```

**Required**

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

### Accessing the Raw Value

associatedtype RawValue

The raw type that can be used to represent all values of the conforming type.

**Required**

