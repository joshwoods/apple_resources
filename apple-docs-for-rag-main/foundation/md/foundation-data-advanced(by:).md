

- Foundation
- Data
-  advanced(by:) 

Instance Method

# advanced(by:)

Returns a new data buffer created by removing the given number of bytes from the front of the original buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func advanced(by amount: Int) -> Data
```

## Parameters 

`amount`  

The number of bytes to strip from the input data buffer. The value must be less than the original data buffer’s length.

## Return Value

A newly created data buffer that is shorter by the given amount than the original.

## See Also

### Excluding Bytes

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func dropFirst(Int) -> Self.SubSequence

Returns a subsequence containing all but the given number of initial elements.

func drop(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

