

- Create ML
- MLDataColumn
-  max() 

Instance Method

# max()

Returns the element with the highest value in a column of doubles.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func max() -> Double?
```

Available when `Element` is `Double`.

## Return Value

A Double; otherwise `nil` if the column is empty or invalid.

## See Also

### Getting the min and max element values

func min() -> Int?

Returns the element with the lowest value in a column of integers.

func min() -> Double?

Returns the element with the lowest value in a column of doubles.

func max() -> Int?

Returns the element with the highest value in a column of integers.

