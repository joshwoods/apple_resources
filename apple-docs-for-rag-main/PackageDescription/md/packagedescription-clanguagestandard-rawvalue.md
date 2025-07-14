

- PackageDescription
- CLanguageStandard
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

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

### Accessing the Raw Value

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

