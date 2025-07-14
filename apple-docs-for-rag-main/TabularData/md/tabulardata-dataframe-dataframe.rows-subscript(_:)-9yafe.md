

- TabularData
- DataFrame
- DataFrame.Rows
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(r: R) -> Self.SubSequence where R : RangeExpression, Self.Index == R.Bound { get set }
```

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

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

func joined() -> FlattenSequence&lt;Self>

Returns the elements of this sequence of sequences, concatenated.

func joined&lt;Separator>(separator: Separator) -> JoinedSequence&lt;Self>

Returns the concatenated elements of this sequence of sequences, inserting the given separator between each element.

subscript(Range&lt;Self.Index>) -> Slice&lt;Self>

Accesses a contiguous subrange of the collection’s elements.

Deprecated

subscript&lt;R>(R) -> Self.SubSequence

Accesses the contiguous subrange of the collection’s elements specified by a range expression.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

