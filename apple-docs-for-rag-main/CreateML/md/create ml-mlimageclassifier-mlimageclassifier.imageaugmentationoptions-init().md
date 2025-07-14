

- Create ML
- MLImageClassifier
- MLImageClassifier.ImageAugmentationOptions
-  init() 

Initializer

# init()

Creates an empty option set.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
init()
```

Available when `RawValue` conforms to `FixedWidthInteger`.

## Discussion

This initializer creates an option set with a raw value of zero.

## See Also

### Creating augmentation options

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(rawValue: Int)

Creates an augmentation set with the given raw value.

let rawValue: Int

The corresponding value of the raw type.

