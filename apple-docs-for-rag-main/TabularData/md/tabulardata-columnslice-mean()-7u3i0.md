

- TabularData
- ColumnSlice
-  mean() 

Instance Method

# mean()

Returns the mean average of the floating-point slice’s elements, ignoring missing elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func mean() -> ColumnSlice.Element
```

Available when `WrappedElement` conforms to `FloatingPoint`.

## See Also

### Getting Statistical Values

func sum() -> WrappedElement

Returns the sum of the column slice’s elements, ignoring missing elements.

func min() -> ColumnSlice&lt;WrappedElement>.Element

Returns the element with the lowest value, ignoring missing elements.

func max() -> ColumnSlice&lt;WrappedElement>.Element

Returns the element with the highest value, ignoring missing elements.

func mean() -> Double?

Returns the mean average of the integer slice’s elements, ignoring missing elements.

func standardDeviation(deltaDegreesOfFreedom: Int) -> Double?

Returns the standard deviation of the integer column slice’s elements, ignoring missing elements.

func standardDeviation(deltaDegreesOfFreedom: Int) -> ColumnSlice&lt;WrappedElement>.Element

Returns the standard deviation of the floating-point column slice’s elements, ignoring missing elements.

