

- Create ML
- MLActionClassifier
- MLActionClassifier.VideoAugmentationOptions
-  init(\_:) 

Initializer

# init(\_:)

Creates a new set from a finite sequence of items.

Create MLSwiftmacOS 10.14+

``` source
init(_ sequence: S) where S : Sequence, Self.Element == S.Element
```

## Parameters 

`sequence`  

The elements to use as members of the new set.

## Discussion

Use this initializer to create a new set from an existing sequence, like an array or a range:

```
let validIndices = Set(0..

## See Also

### Creating augmentation options

init(rawValue: Int)

Creates a video augmentation option set from a raw value.

init()

Creates an empty option set.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

