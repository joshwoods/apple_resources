

- Create ML
- MLImageClassifier
- MLImageClassifier.ImageAugmentationOptions
-  rawValue 

Instance Property

# rawValue

The corresponding value of the raw type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

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

### Creating augmentation options

init()

Creates an empty option set.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(rawValue: Int)

Creates an augmentation set with the given raw value.

