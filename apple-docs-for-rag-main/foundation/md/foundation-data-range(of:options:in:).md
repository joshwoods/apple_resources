

- Foundation
- Data
-  range(of:options:in:) 

Instance Method

# range(of:options:in:)

Finds the range of the specified data as a subsequence of this data, if it exists.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func range(
    of dataToFind: Data,
    options: Data.SearchOptions = [],
    in range: Range? = nil
) -> Range?
```

## Parameters 

`dataToFind`  

The data to be searched for.

`options`  

Options for the search. Default value is `[]`.

`range`  

The range of this data in which to perform the search. Default value is `nil`, which means the entire content of this data.

## Return Value

A `Range` specifying the location of the found data, or nil if a match could not be found.

## Discussion

Precondition: `range` must be in the bounds of the Data.

## See Also

### Finding Bytes

func first(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func max() -> Self.Element?

Returns the maximum element in the sequence.

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

func min() -> Self.Element?

Returns the minimum element in the sequence.

func min(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the minimum element in the sequence, using the given predicate as the comparison between elements.

typealias SearchOptions

Options that control a data search operation.

