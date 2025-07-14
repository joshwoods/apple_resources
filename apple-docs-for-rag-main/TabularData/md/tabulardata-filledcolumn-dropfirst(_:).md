

- TabularData
- FilledColumn
-  dropFirst(\_:) 

Instance Method

# dropFirst(\_:)

Returns a subsequence containing all but the given number of initial elements.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func dropFirst(_ k: Int = 1) -> Self.SubSequence
```

## Parameters 

`k`  

The number of elements to drop from the beginning of the collection. `k` must be greater than or equal to zero.

## Return Value

A subsequence starting after the specified number of elements.

## Discussion

If the number of elements to drop exceeds the number of elements in the collection, the result is an empty subsequence.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.dropFirst(2))
// Prints "[3, 4, 5]"
print(numbers.dropFirst(10))
// Prints "[]"
```

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the number of elements to drop from the beginning of the collection.

## See Also

### Generating Subsequences

func drop(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

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

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

func joined() -> FlattenSequence&lt;Self>

Returns the elements of this sequence of sequences, concatenated.

func joined&lt;Separator>(separator: Separator) -> JoinedSequence&lt;Self>

Returns the concatenated elements of this sequence of sequences, inserting the given separator between each element.

func joined(separator: String) -> String

Returns a new string by concatenating the elements of the sequence, adding the given separator between each element.

func joined(separator: String) -> String

Returns a new string by concatenating the elements of the sequence, adding the given separator between each element.

