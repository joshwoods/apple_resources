

- Metal
- MTLArgumentEncoder
-  setIntersectionFunctionTable(\_:index:) 

Instance Method

# setIntersectionFunctionTable(\_:index:)

Encodes a reference to a ray-tracing intersection-function table into the argument buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func setIntersectionFunctionTable(
    _ intersectionFunctionTable: (any MTLIntersectionFunctionTable)?,
    index: Int
)
```

**Required**

## Parameters 

`intersectionFunctionTable`  

An intersection-function table the method encodes.

`index`  

An index of an intersection-function table within the argument buffer. The value corresponds to either the index ID of a declaration in Metal Shading Language (MSL) or the index property of an MTLArgumentDescriptor instance.

## See Also

### Encoding Function Tables

func setVisibleFunctionTable((any MTLVisibleFunctionTable)?, index: Int)

Encodes a reference to a visible-function table into the argument buffer.

**Required**

func setIntersectionFunctionTables([(any MTLIntersectionFunctionTable)?], range: Range&lt;Int>)

Encodes references to an array of ray-tracing intersection-function tables into the argument buffer.

func setVisibleFunctionTables([(any MTLVisibleFunctionTable)?], range: Range&lt;Int>)

Encodes references to an array of ray-tracing intersection-function tables into the argument buffer.

