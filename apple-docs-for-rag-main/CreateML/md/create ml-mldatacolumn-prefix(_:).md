

- Create ML
- MLDataColumn
-  prefix(\_:) 

Instance Method

# prefix(\_:)

Creates a subset of the column, given a number of initial elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func prefix(_ maxLength: Int = 10) -> MLDataColumn
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Parameters 

`maxLength`  

An integer that limits the number of elements to use from the beginning of the column. The default value is `10`.

## Return Value

A new column.

## See Also

### Selecting elements to generate a column

subscript(Range&lt;Int>) -> MLDataColumn&lt;Element>

Creates a subset of the column, given a range of elements.

subscript&lt;R>(R) -> MLDataColumn&lt;Element>

Creates a subset of the column, given a range expression of elements.

func suffix(Int) -> MLDataColumn&lt;Element>

Creates a subset of the column, given a number of final elements.

