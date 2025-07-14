

- Metal
-  MTLVisibleFunctionTable 

Protocol

# MTLVisibleFunctionTable

A table of shader functions visible to your app that you can pass into compute commands to customize the behavior of a shader.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLVisibleFunctionTable : MTLResource
```

## Topics

### Setting a Table Entry

func setFunction((any MTLFunctionHandle)?, index: Int)

Sets a table entry to point to a callable function.

**Required**

func setFunctions([(any MTLFunctionHandle)?], range: Range&lt;Int>)

Sets a range of table entries to point to an array of callable functions.

### Instance Properties

var gpuResourceID: MTLResourceID

**Required**

## Relationships

### Inherits From

- MTLAllocation
- MTLResource
- NSObjectProtocol

## See Also

### Shader Functions

class MTLFunctionDescriptor

A description of a function object to create.

protocol MTLFunction

An object that represents a public shader function in a Metal library.

protocol MTLFunctionHandle

An object representing a function that you can add to a visible function table.

class MTLVisibleFunctionTableDescriptor

A specification of how to create a visible function table.

class MTLIntersectionFunctionDescriptor

A description of an intersection function that performs an intersection test.

class MTLIntersectionFunctionTableDescriptor

A specification of how to create an intersection function table.

protocol MTLIntersectionFunctionTable

A table of intersection functions that Metal calls to perform ray-tracing intersection tests.

