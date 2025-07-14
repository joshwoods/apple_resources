

- TabularData
- DiscontiguousColumnSlice
-  firstIndex(where:) 

Instance Method

# firstIndex(where:)

Returns the first index in which an element of the collection satisfies the given predicate.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func firstIndex(where predicate: (Self.Element) throws -> Bool) rethrows -> Self.Index?
```

## Parameters 

`predicate`  

A closure that takes an element as its argument and returns a Boolean value that indicates whether the passed element represents a match.

## Return Value

The index of the first element for which `predicate` returns `true`. If no elements in the collection satisfy the given predicate, returns `nil`.

## Discussion

You can use the predicate to find an element of a type that doesn’t conform to the `Equatable` protocol or to find an element that matches particular criteria. Here’s an example that finds a student name that begins with the letter “A”:

```
let students = ["Kofi", "Abena", "Peter", "Kweku", "Akosua"]
if let i = students.firstIndex(where: { $0.hasPrefix("A") }) {
    print("\(students[i]) starts with 'A'!")
}
// Prints "Abena starts with 'A'!"
```

Complexity

O(*n*), where *n* is the length of the collection.

## See Also

### Retrieving an Index

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

