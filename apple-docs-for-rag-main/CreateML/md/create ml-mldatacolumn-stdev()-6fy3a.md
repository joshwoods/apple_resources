

- Create ML
- MLDataColumn
-  stdev() 

Instance Method

# stdev()

Standard deviation of the Elements in the MLDataColumn.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 16.0+visionOS 1.0+

``` source
func stdev() -> Double?
```

Available when `Element` is `Int`.

## Return Value

Standard deviation of the Element values in the MLDataColumn. Returns nil if the MLDataColumn is invalid, 0 if the MLDataColumn is empty.

## See Also

### Getting sum, mean, and standard deviation values

func sum() -> Int?

Returns the sum of the elements in a column of integers.

func sum() -> Double?

Returns the sum of the elements in a column of doubles.

func mean() -> Double?

Returns the arithmetic mean of the elements in a column of integers.

func mean() -> Double?

Returns the arithmetic mean of the elements in a column of doubles.

func std() -> Double?

Returns the standard deviation of the elements in a column of integers.

func std() -> Double?

Returns the standard deviation of the elements in a column of doubles.

func stdev() -> Double?

Returns the standard deviation of the elements in a column of doubles.

