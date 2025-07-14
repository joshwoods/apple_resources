

- Create ML
- MLUntypedColumn
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Creates a subset of the column by masking its elements with another untyped column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(mask: MLUntypedColumn) -> MLUntypedColumn { get }
```

## Parameters 

`mask`  

An untyped column indicating whether elements should be removed (a default value) or included (any nondefault value) in the derived column.

## Return Value

A new column.

## Overview

Use this untyped column–based subscript to create a new column by masking a subset of the elements. The derived column will not include elements where `mask` contains a default value for its underlying type, such as:

- `0` in untyped `Int` columns

- `0.0` in untyped `Double` columns

- An empty string in untyped `String` columns

The derived column includes elements where the masking column has any other (nondefault) value.

See subscript(_:) from MLDataTable for an example.

## See Also

### Masking elements to generate an untyped column

subscript(MLDataColumn&lt;Bool>) -> MLUntypedColumn

Creates a subset of the column by masking its elements with a data column of Booleans.

