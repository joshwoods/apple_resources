

- TabularData
- Column
-  standardDeviation(deltaDegreesOfFreedom:) 

Instance Method

# standardDeviation(deltaDegreesOfFreedom:)

Returns the standard deviation of the integer column’s elements, ignoring missing elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func standardDeviation(deltaDegreesOfFreedom: Int = 1) -> Double?
```

Available when `WrappedElement` conforms to `BinaryInteger`.

## Parameters 

`deltaDegreesOfFreedom`  

A nonnegative integer. The method calculates the standard deviation’s divisor by subtracting this parameter from the number of non-`nil` elements (`n - deltaDegreesOfFreedom` where `n` is the number of non-`nil` elements).

## Return Value

The standard deviation; otherwise, `nil` if there are fewer than `deltaDegreesOfFreedom + 1` non-`nil` items in the column.

## See Also

### Getting Statistical Values

func sum() -> WrappedElement

Returns the sum of the column’s elements, ignoring missing elements.

func min() -> Column&lt;WrappedElement>.Element

Returns the element with the lowest value, ignoring missing elements.

func max() -> Column&lt;WrappedElement>.Element

Returns the element with the highest value, ignoring missing elements.

func mean() -> Double?

Returns the mean average of the integer column’s elements, ignoring missing elements.

func mean() -> Column&lt;WrappedElement>.Element

Returns the mean average of the floating-point column’s elements, ignoring missing elements.

func standardDeviation(deltaDegreesOfFreedom: Int) -> Column&lt;WrappedElement>.Element

Returns the standard deviation of the floating-point column’s elements, ignoring missing elements.

