

- Swift
- Int
-  subtractingReportingOverflow(\_:) 

Instance Method

# subtractingReportingOverflow(\_:)

Returns the difference obtained by subtracting the given value from this value, along with a Boolean value indicating whether overflow occurred in the operation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func subtractingReportingOverflow(_ other: Int) -> (partialValue: Int, overflow: Bool)
```

## Return Value

A tuple containing the result of the subtraction along with a Boolean value indicating whether overflow occurred. If the `overflow` component is `false`, the `partialValue` component contains the entire difference. If the `overflow` component is `true`, an overflow occurred and the `partialValue` component contains the truncated result of `rhs` subtracted from this value.

## See Also

### Performing Calculations with Overflow

func addingReportingOverflow(Int) -> (partialValue: Int, overflow: Bool)

Returns the sum of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func multipliedReportingOverflow(by: Int) -> (partialValue: Int, overflow: Bool)

Returns the product of this value and the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func dividedReportingOverflow(by: Int) -> (partialValue: Int, overflow: Bool)

Returns the quotient obtained by dividing this value by the given value, along with a Boolean value indicating whether overflow occurred in the operation.

func remainderReportingOverflow(dividingBy: Int) -> (partialValue: Int, overflow: Bool)

Returns the remainder after dividing this value by the given value, along with a Boolean value indicating whether overflow occurred during division.

