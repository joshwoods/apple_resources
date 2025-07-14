

- TabularData
- DataFrame
- DataFrame.Slice
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Generates a data frame slice that includes the columns in a sequence of column names.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(columnNames: S) -> DataFrame.Slice where S : Sequence, S.Element == String { get }
```

## Parameters 

`columnNames`  

A sequence of column names.

## Return Value

A new data frame slice.

## See Also

### Creating a Slice by Selecting Multiple Columns

func selecting&lt;S>(columnNames: S) -> DataFrame.Slice

Generates a data frame slice that includes the columns you select with a sequence of names.

func selecting(columnNames: String...) -> DataFrame.Slice

Generates a data frame slice that includes the columns you select with a list of names.

