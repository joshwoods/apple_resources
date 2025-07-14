

- TabularData
- FilledColumn
-  standardDeviation(deltaDegreesOfFreedom:) 

Instance Method

# standardDeviation(deltaDegreesOfFreedom:)

Returns the standard deviation of the floating-point column’s elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func standardDeviation(deltaDegreesOfFreedom: Int = 1) -> FilledColumn.Element?
```

Available when `Base` conforms to `OptionalColumnProtocol` and `Base.WrappedElement` conforms to `FloatingPoint`.

## Parameters 

`deltaDegreesOfFreedom`  

A nonnegative integer. The method calculates the standard deviation’s divisor by subtracting this parameter from the number of non-`nil` elements (`n - deltaDegreesOfFreedom` where `n` is the number of non-`nil` elements).

## Return Value

The standard deviation; otherwise, `nil` if there are fewer than `deltaDegreesOfFreedom + 1` non-`nil` items in the column.

## See Also

### Getting Statistical Values

func sum() -> FilledColumn&lt;Base>.Element

Returns the sum of the integer column’s elements.

func sum() -> FilledColumn&lt;Base>.Element

Returns the sum of the floating-point column’s elements.

func min() -> FilledColumn&lt;Base>.Element?

Returns the element with the lowest value.

func max() -> FilledColumn&lt;Base>.Element?

Returns the element with the highest value.

func mean() -> Double?

Returns the mean average of the integer column’s elements.

func mean() -> FilledColumn&lt;Base>.Element?

Returns the mean average of the floating-point column’s elements.

func standardDeviation(deltaDegreesOfFreedom: Int) -> Double?

Returns the standard deviation of the integer column’s elements.

