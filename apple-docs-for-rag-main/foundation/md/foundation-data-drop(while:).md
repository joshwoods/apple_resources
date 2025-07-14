

- Foundation
- Data
-  drop(while:) 

Instance Method

# drop(while:)

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func drop(while predicate: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence
```

## Parameters 

`predicate`  

A closure that takes an element of the sequence as its argument and returns `true` if the element should be skipped or `false` if it should be included. Once the predicate returns `false` it will not be called again.

## Discussion

Complexity

O(*n*), where *n* is the length of the collection.

## See Also

### Excluding Bytes

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func dropFirst(Int) -> Self.SubSequence

Returns a subsequence containing all but the given number of initial elements.

func advanced(by: Int) -> Data

Returns a new data buffer created by removing the given number of bytes from the front of the original buffer.

