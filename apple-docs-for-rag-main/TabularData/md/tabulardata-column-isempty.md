

- TabularData
- Column
-  isEmpty 

Instance Property

# isEmpty

A Boolean value indicating whether the collection is empty.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var isEmpty: Bool { get }
```

## Discussion

When you need to check whether your collection is empty, use the `isEmpty` property instead of checking that the `count` property is equal to zero. For collections that don’t conform to `RandomAccessCollection`, accessing the `count` property iterates through the elements of the collection.

```
let horseName = "Silver"
if horseName.isEmpty {
    print("My horse has no name.")
} else {
    print("Hi ho, \(horseName)!")
}
// Prints "Hi ho, Silver!")
```

Complexity

O(1)

## See Also

### Inspecting a Column

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

func makeIterator() -> IndexingIterator&lt;Self>

Returns an iterator over the elements of the collection.

