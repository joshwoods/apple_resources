

- TabularData
- DataFrame
- DataFrame.Slice
-  prefix(upTo:) 

Instance Method

# prefix(upTo:)

Returns a new slice that contains the initial elements of the original slice up to, but not including, the element at a position.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func prefix(upTo position: Int) -> DataFrame.Slice
```

## Parameters 

`position`  

A valid index to an element in the slice.

## Return Value

A new slice of the underlying data frame.

## See Also

### Creating a Slice by Selecting Rows

func prefix(Int) -> DataFrame.Slice

Returns a new slice that contains the initial elements of the original slice.

func prefix(through: Int) -> DataFrame.Slice

Returns a new slice that contains the initial elements of the original slice up to and including the element at a position.

func suffix(Int) -> DataFrame.Slice

Returns a new slice that contains the final elements of the original slice.

func suffix(from: Int) -> DataFrame.Slice

Returns a new slice that contains the final elements of the original slice beginning with the element at a position.

