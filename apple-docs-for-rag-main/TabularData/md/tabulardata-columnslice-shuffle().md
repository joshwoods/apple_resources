

- TabularData
- ColumnSlice
-  shuffle() 

Instance Method

# shuffle()

Shuffles the collection in place.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

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

## See Also

### Shuffling a Column Slice

func shuffle&lt;T>(using: inout T)

Shuffles the collection in place, using the given generator as a source for randomness.

