

- Metal
- MTLArgumentEncoder
-  setVisibleFunctionTables(\_:range:) 

Instance Method

# setVisibleFunctionTables(\_:range:)

Encodes references to an array of ray-tracing intersection-function tables into the argument buffer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 16.0+visionOS

``` source
func setVisibleFunctionTables(
    _ visibleFunctionTables: [(any MTLVisibleFunctionTable)?],
    range: Range
)
```

## Parameters 

`visibleFunctionTables`  

An array of visible-function tables the method encodes.

`range`  

A range of indices within the argument buffer for each element in `visibleFunctionTables`. The values correspond to either the index IDs of declarations in Metal Shading Language (MSL) or the index property of MTLArgumentDescriptor instances.

## See Also

### Encoding Function Tables

func setVisibleFunctionTable((any MTLVisibleFunctionTable)?, index: Int)

Encodes a reference to a visible-function table into the argument buffer.

**Required**

func setIntersectionFunctionTable((any MTLIntersectionFunctionTable)?, index: Int)

Encodes a reference to a ray-tracing intersection-function table into the argument buffer.

**Required**

func setIntersectionFunctionTables([(any MTLIntersectionFunctionTable)?], range: Range&lt;Int>)

Encodes references to an array of ray-tracing intersection-function tables into the argument buffer.

