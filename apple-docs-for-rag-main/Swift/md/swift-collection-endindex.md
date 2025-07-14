

- Swift
- Collection
-  endIndex 

Instance Property

# endIndex

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var endIndex: Self.Index { get }
```

**Required**

## Discussion

When you need a range that includes the last element of a collection, use the half-open range operator (`..

```
let numbers = [10, 20, 30, 40, 50]
if let index = numbers.firstIndex(of: 30) {
    print(numbers[index ..

If the collection is empty, `endIndex` is equal to `startIndex`.

## See Also

### Manipulating Indices

var startIndex: Self.Index

The position of the first element in a nonempty collection.

**Required**

var indices: Self.Indices

The indices that are valid for subscripting the collection, in ascending order.

**Required** Default implementations provided.

func index(after: Self.Index) -> Self.Index

Returns the position immediately after the given index.

**Required** Default implementation provided.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

