

- TabularData
- AnyColumnProtocol
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Retrieves an element at a position in the column type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(position: Int) -> Any? { get }
```

**Required**

## Parameters 

`position`  

A valid index in the column type.

## See Also

### Retrieving Elements

subscript(Range&lt;Int>) -> AnyColumnSlice

Retrieves a contiguous subrange of the column type’s elements.

**Required**

