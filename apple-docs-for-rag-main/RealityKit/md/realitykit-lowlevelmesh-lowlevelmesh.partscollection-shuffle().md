

- RealityKit
- LowLevelMesh
- LowLevelMesh.PartsCollection
-  shuffle() 

Instance Method

# shuffle()

Shuffles the collection in place.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
mutating func shuffle()
```

Available when `Self` conforms to `RandomAccessCollection`.

## Discussion

Use the `shuffle()` method to randomly reorder the elements of an array.

```
var names = ["Alejandro", "Camila", "Diego", "Luciana", "Luis", "Sofía"]
names.shuffle()
// names == ["Luis", "Camila", "Luciana", "Sofía", "Alejandro", "Diego"]
```

This method is equivalent to calling `shuffle(using:)`, passing in the system’s default random generator.

Complexity

O(*n*), where *n* is the length of the collection.

