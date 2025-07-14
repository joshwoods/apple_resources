

- Create ML
- MLDataTable
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Creates a subset of the table given a sequence of column names.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(columnNames: S) -> MLDataTable where S : Sequence, S.Element == String { get }
```

## Parameters 

`columnNames`  

A sequence of names indicating which columns to includein the new data table.

## Return Value

A new data table.

