

- ManagedSettings
- SafariSettings
- SafariSettings.CookiePolicy
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

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

