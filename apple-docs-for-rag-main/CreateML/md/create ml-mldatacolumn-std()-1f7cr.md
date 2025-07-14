

- Create ML
- MLDataColumn
-  std() 

Instance Method

# std()

Returns the standard deviation of the elements in a column of doubles.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOS 10.14–10.15DeprecatedvisionOS 1.0+

``` source
func std() -> Double?
```

Available when `Element` is `Double`.

## Return Value

A Double; otherwise `nil` if the column is invalid.

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

func stdev() -> Double?

Returns the standard deviation of the elements in a column of doubles.

func stdev() -> Double?

Standard deviation of the Elements in the MLDataColumn.

