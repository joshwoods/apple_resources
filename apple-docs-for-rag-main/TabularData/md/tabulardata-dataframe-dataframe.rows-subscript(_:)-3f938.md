

- TabularData
- DataFrame
- DataFrame.Rows
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a row at an index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(position: Int) -> DataFrame.Row { get set }
```

## Parameters 

`position`  

A valid index to a row in the collection.

## See Also

### Accessing Elements

subscript(Range&lt;Int>) -> DataFrame.Rows

Returns a row collection from an index range.

