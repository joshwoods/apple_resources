

- Foundation
- Data
-  sort(by:) 

Instance Method

# sort(by:)

Sorts the collection in place, using the given predicate as the comparison between elements.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func sort(by areInIncreasingOrder: (Self.Element, Self.Element) throws -> Bool) rethrows
```

Available when `Self` conforms to `RandomAccessCollection`.

## Parameters 

`areInIncreasingOrder`  

A predicate that returns `true` if its first argument should be ordered before its second argument; otherwise, `false`. If `areInIncreasingOrder` throws an error during the sort, the elements may be in a different order, but none will be lost.

## Discussion

When you want to sort a collection of elements that don’t conform to the `Comparable` protocol, pass a closure to this method that returns `true` when the first element should be ordered before the second.

In the following example, the closure provides an ordering for an array of a custom enumeration that describes an HTTP response. The predicate orders errors before successes and sorts the error responses by their error code.

```
enum HTTPResponse {
    case ok
    case error(Int)
}

var responses: [HTTPResponse] = [.error(500), .ok, .ok, .error(404), .error(403)]
responses.sort {
    switch ($0, $1) {
    // Order errors by code
    case let (.error(aCode), .error(bCode)):
        return aCode 

Alternatively, use this method to sort a collection of elements that do conform to `Comparable` when you want the sort to be descending instead of ascending. Pass the greater-than operator (`>`) operator as the predicate.

```
var students = ["Kofi", "Abena", "Peter", "Kweku", "Akosua"]
students.sort(by: >)
print(students)
// Prints "["Peter", "Kweku", "Kofi", "Akosua", "Abena"]"
```

`areInIncreasingOrder` must be a *strict weak ordering* over the elements. That is, for any elements `a`, `b`, and `c`, the following conditions must hold:

- `areInIncreasingOrder(a, a)` is always `false`. (Irreflexivity)

- If `areInIncreasingOrder(a, b)` and `areInIncreasingOrder(b, c)` are both `true`, then `areInIncreasingOrder(a, c)` is also `true`. (Transitive comparability)

- Two elements are *incomparable* if neither is ordered before the other according to the predicate. If `a` and `b` are incomparable, and `b` and `c` are incomparable, then `a` and `c` are also incomparable. (Transitive incomparability)

The sorting algorithm is guaranteed to be stable. A stable sort preserves the relative order of elements for which `areInIncreasingOrder` does not establish an order.

Complexity

O(*n* log *n*), where *n* is the length of the collection.

## See Also

### Sorting Bytes

func sorted() -> [Self.Element]

Returns the elements of the sequence, sorted.

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func reversed() -> ReversedCollection&lt;Self>

Returns a view presenting the elements of the collection in reverse order.

