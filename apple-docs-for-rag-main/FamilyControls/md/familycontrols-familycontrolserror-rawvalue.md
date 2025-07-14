

- FamilyControls
- FamilyControlsError
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+

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

