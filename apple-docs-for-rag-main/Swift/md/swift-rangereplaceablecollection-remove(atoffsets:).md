

- Swift
- RangeReplaceableCollection
-  remove(atOffsets:) 

Instance Method

# remove(atOffsets:)

Removes all the elements at the specified offsets from the collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func remove(atOffsets offsets: IndexSet)
```

Available when `Self` conforms to `MutableCollection`.

## Discussion

Complexity

O(*n*) where *n* is the length of the collection.

