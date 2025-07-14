

- MusicKit
- MusicSubscriptionOffer
- MusicSubscriptionOffer.MessageIdentifier
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

MusicKitSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
let rawValue: String
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

