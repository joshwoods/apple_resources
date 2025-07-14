

- Swift
- ArraySlice
-  shuffle() 

Instance Method

# shuffle()

Shuffles the collection in place.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

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

