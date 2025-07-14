

- Foundation
- Data
-  Data.SearchOptions 

Type Alias

# Data.SearchOptions

Options that control a data search operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias SearchOptions = NSData.SearchOptions
```

## See Also

### Related Documentation

struct SearchOptions

Options for method used to search data objects.

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

func range(of: Data, options: Data.SearchOptions, in: Range&lt;Data.Index>?) -> Range&lt;Data.Index>?

Finds the range of the specified data as a subsequence of this data, if it exists.

