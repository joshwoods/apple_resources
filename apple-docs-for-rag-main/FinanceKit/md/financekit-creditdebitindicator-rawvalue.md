

- FinanceKit
- CreditDebitIndicator
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 17.4+iPadOS 17.4+

``` source
var rawValue: Int16 { get }
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

