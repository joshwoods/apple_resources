

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.VideoAugmentationOptions
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
let rawValue: Int
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

### Inspecting an Augmentation

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

func contains(Self) -> Bool

Returns a Boolean value that indicates whether a given element is a member of the option set.

