

- Swift
- EmptyCollection
-  reverse() 

Instance Method

# reverse()

Reverses the elements of the collection in place.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func reverse()
```

Available when `Self` conforms to `BidirectionalCollection`.

## Discussion

The following example reverses the elements of an array of characters:

```
var characters: [Character] = ["C", "a", "f", "é"]
characters.reverse()
print(characters)
// Prints "["é", "f", "a", "C"]"
```

Complexity

O(*n*), where *n* is the number of elements in the collection.

