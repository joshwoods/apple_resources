

- Create ML
- MLDataTable
-  subscript(\_:\_:) 

Instance Subscript

# subscript(\_:\_:)

Retrieves a column with the specified name and type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(columnName: String, columnType: T.Type) -> MLDataColumn? where T : MLDataValueConvertible { get }
```

## Parameters 

`columnName`  

The name of the column to extract.

`columnType`  

The underlying type of the column’s content.

## Return Value

A new MLDataColumn with the specified name and type, if it exists; otherwise `nil`.

## Overview

Use this subscript to get a typed MLDataColumn, which is easier to work with than a MLUntypedColumn returned from subscript(_:).

## See Also

### Accessing columns

subscript&lt;Element>(String) -> MLDataColumn&lt;Element>

Retrieves or adds a typed column with the specified name.

subscript(String) -> MLUntypedColumn

Retrieves or adds an untyped column with the specified name.

