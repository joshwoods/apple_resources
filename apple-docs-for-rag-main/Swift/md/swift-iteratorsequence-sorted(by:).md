

- Swift
- IteratorSequence
-  sorted(by:) 

Instance Method

# sorted(by:)

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sorted(by areInIncreasingOrder: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]
```

## Parameters 

`areInIncreasingOrder`  

A predicate that returns `true` if its first argument should be ordered before its second argument; otherwise, `false`.

## Return Value

A sorted array of the sequence’s elements.

## Discussion

When you want to sort a sequence of elements that don’t conform to the `Comparable` protocol, pass a predicate to this method that returns `true` when the first element should be ordered before the second. The elements of the resulting array are ordered according to the given predicate.

In the following example, the predicate provides an ordering for an array of a custom `HTTPResponse` type. The predicate orders errors before successes and sorts the error responses by their error code.

```
enum HTTPResponse {
    case ok
    case error(Int)
}

let responses: [HTTPResponse] = [.error(500), .ok, .ok, .error(404), .error(403)]
let sortedResponses = responses.sorted {
    switch ($0, $1) {
    // Order errors by code
    case let (.error(aCode), .error(bCode)):
        return aCode 

You also use this method to sort elements that conform to the `Comparable` protocol in descending order. To sort your sequence in descending order, pass the greater-than operator (`>`) as the `areInIncreasingOrder` parameter.

```
let students: Set = ["Kofi", "Abena", "Peter", "Kweku", "Akosua"]
let descendingStudents = students.sorted(by: >)
print(descendingStudents)
// Prints "["Peter", "Kweku", "Kofi", "Akosua", "Abena"]"
```

Calling the related `sorted()` method is equivalent to calling this method and passing the less-than operator (`

```
print(students.sorted())
// Prints "["Abena", "Akosua", "Kofi", "Kweku", "Peter"]"
print(students.sorted(by: 

The predicate must be a *strict weak ordering* over the elements. That is, for any elements `a`, `b`, and `c`, the following conditions must hold:

- `areInIncreasingOrder(a, a)` is always `false`. (Irreflexivity)

- If `areInIncreasingOrder(a, b)` and `areInIncreasingOrder(b, c)` are both `true`, then `areInIncreasingOrder(a, c)` is also `true`. (Transitive comparability)

- Two elements are *incomparable* if neither is ordered before the other according to the predicate. If `a` and `b` are incomparable, and `b` and `c` are incomparable, then `a` and `c` are also incomparable. (Transitive incomparability)

The sorting algorithm is guaranteed to be stable. A stable sort preserves the relative order of elements for which `areInIncreasingOrder` does not establish an order.

Complexity

O(*n* log *n*), where *n* is the length of the sequence.

