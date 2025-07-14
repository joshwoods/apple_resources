

- TabularData
- AnyColumnProtocol
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Retrieves a contiguous subrange of the column type’s elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(range: Range) -> AnyColumnSlice { get }
```

**Required**

## Parameters 

`range`  

An integer range of valid indices in the column.

## See Also

### Retrieving Elements

subscript(Int) -> Any?

Retrieves an element at a position in the column type.

**Required**

