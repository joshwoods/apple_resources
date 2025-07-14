

- TabularData
- AnyColumn
-  suffix(from:) 

Instance Method

# suffix(from:)

Returns a subsequence from the specified position to the end of the collection.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func suffix(from start: Self.Index) -> Self.SubSequence
```

## Parameters 

`start`  

The index at which to start the resulting subsequence. `start` must be a valid index of the collection.

## Return Value

A subsequence starting at the `start` position.

## Discussion

The following example searches for the index of the number `40` in an array of integers, and then prints the suffix of the array starting at that index:

```
let numbers = [10, 20, 30, 40, 50, 60]
if let i = numbers.firstIndex(of: 40) {
    print(numbers.suffix(from: i))
}
// Prints "[40, 50, 60]"
```

Passing the collection’s `endIndex` as the `start` parameter results in an empty subsequence.

```
print(numbers.suffix(from: numbers.endIndex))
// Prints "[]"
```

Using the `suffix(from:)` method is equivalent to using a partial range from the index as the collection’s subscript. The subscript notation is preferred over `suffix(from:)`.

```
if let i = numbers.firstIndex(of: 40) {
    print(numbers[i...])
}
// Prints "[40, 50, 60]"
```

Complexity

O(1)

## See Also

### Generating Subsequences

func drop(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

func dropFirst(Int) -> Self.SubSequence

Returns a subsequence containing all but the given number of initial elements.

func prefix(Int) -> Self.SubSequence

Returns a subsequence, up to the specified maximum length, containing the initial elements of the collection.

func prefix(upTo: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection up to, but not including, the specified position.

func prefix(through: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection through the specified position.

func prefix(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence containing the initial elements until `predicate` returns `false` and skipping the remaining elements.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

