

- RealityKit
- LowLevelMesh
- LowLevelMesh.PartsCollection
-  shuffle(using:) 

Instance Method

# shuffle(using:)

Shuffles the collection in place, using the given generator as a source for randomness.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
mutating func shuffle(using generator: inout T) where T : RandomNumberGenerator
```

Available when `Self` conforms to `RandomAccessCollection`.

## Parameters 

`generator`  

The random number generator to use when shuffling the collection.

## Discussion

You use this method to randomize the elements of a collection when you are using a custom random number generator. For example, you can use the `shuffle(using:)` method to randomly reorder the elements of an array.

```
var names = ["Alejandro", "Camila", "Diego", "Luciana", "Luis", "Sofía"]
names.shuffle(using: &myGenerator)
// names == ["Sofía", "Alejandro", "Camila", "Luis", "Diego", "Luciana"]
```

Complexity

O(*n*), where *n* is the length of the collection.

Note

The algorithm used to shuffle a collection may change in a future version of Swift. If you’re passing a generator that results in the same shuffled order each time you run your program, that sequence may change when your program is compiled using a different version of Swift.

