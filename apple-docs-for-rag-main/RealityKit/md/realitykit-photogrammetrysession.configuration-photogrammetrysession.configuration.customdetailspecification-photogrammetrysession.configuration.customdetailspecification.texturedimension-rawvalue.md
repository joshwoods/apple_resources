

- RealityKit
- PhotogrammetrySession
- 
  - PhotogrammetrySession
- PhotogrammetrySession.Configuration
- PhotogrammetrySession.Configuration.CustomDetailSpecification
- PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureDimension
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

Mac Catalyst 17.0+macOS 14.0+

``` source
var rawValue: UInt { get }
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

