

- Foundation
- Data
-  resetBytes(in:) 

Instance Method

# resetBytes(in:)

Replaces the contents of the buffer at the given range with zeroes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func resetBytes(in range: R) where R : RangeExpression, Self.Index == R.Bound
```

## Discussion

A default implementation is given in terms of `replaceSubrange(_:with:)`.

