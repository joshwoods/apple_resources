

- Foundation
- Data
-  firstRange(of:in:) 

Instance Method

# firstRange(of:in:)

Returns the first found range of the given data buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func firstRange(
    of data: D,
    in range: R
) -> Range? where D : DataProtocol, R : RangeExpression, Self.Index == R.Bound
```

## Discussion

A default implementation is given in terms of `self.regions`.

