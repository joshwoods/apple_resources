

- Swift
- UInt128
-  multipliedReportingOverflow(by:) 

Instance Method

# multipliedReportingOverflow(by:)

Returns the product of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func multipliedReportingOverflow(by other: UInt128) -> (partialValue: UInt128, overflow: Bool)
```

## Return Value

A tuple containing the result of the multiplication along with a Boolean value indicating whether overflow occurred. If the `overflow` component is `false`, the `partialValue` component contains the entire product. If the `overflow` component is `true`, an overflow occurred and the `partialValue` component contains the truncated product of this value and `rhs`.

