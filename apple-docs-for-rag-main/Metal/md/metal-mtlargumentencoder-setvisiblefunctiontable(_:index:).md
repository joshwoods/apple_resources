

- Metal
- MTLArgumentEncoder
-  setVisibleFunctionTable(\_:index:) 

Instance Method

# setVisibleFunctionTable(\_:index:)

Encodes a reference to a visible-function table into the argument buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func setVisibleFunctionTable(
    _ visibleFunctionTable: (any MTLVisibleFunctionTable)?,
    index: Int
)
```

**Required**

## Parameters 

`visibleFunctionTable`  

A visible-function table the method encodes.

`index`  

The index of a visible-function table within the argument buffer. The value corresponds to either the index ID of a declaration in Metal Shading Language (MSL) or the index property of an MTLArgumentDescriptor instance.

## See Also

### Encoding Function Tables

func setIntersectionFunctionTable((any MTLIntersectionFunctionTable)?, index: Int)

Encodes a reference to a ray-tracing intersection-function table into the argument buffer.

**Required**

func setIntersectionFunctionTables([(any MTLIntersectionFunctionTable)?], range: Range&lt;Int>)

Encodes references to an array of ray-tracing intersection-function tables into the argument buffer.

func setVisibleFunctionTables([(any MTLVisibleFunctionTable)?], range: Range&lt;Int>)

Encodes references to an array of ray-tracing intersection-function tables into the argument buffer.

