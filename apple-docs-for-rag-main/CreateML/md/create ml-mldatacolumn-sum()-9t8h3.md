

- Create ML
- MLDataColumn
-  sum() 

Instance Method

# sum()

Returns the sum of the elements in a column of integers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func sum() -> Int?
```

Available when `Element` is `Int`.

## Return Value

An Int; otherwise `nil` if the column is invalid.

## See Also

### Getting sum, mean, and standard deviation values

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

func stdev() -> Double?

Standard deviation of the Elements in the MLDataColumn.

