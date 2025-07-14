

- Metal
-  MTLFunctionHandle 

Protocol

# MTLFunctionHandle

An object representing a function that you can add to a visible function table.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLFunctionHandle : NSObjectProtocol
```

## Topics

### Querying Handle Properties

var device: any MTLDevice

The device object that created the shader function.

**Required**

var functionType: MTLFunctionType

The shader function’s type.

**Required**

var name: String

The function’s name.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Shader Functions

class MTLFunctionDescriptor

A description of a function object to create.

protocol MTLFunction

An object that represents a public shader function in a Metal library.

class MTLVisibleFunctionTableDescriptor

A specification of how to create a visible function table.

protocol MTLVisibleFunctionTable

A table of shader functions visible to your app that you can pass into compute commands to customize the behavior of a shader.

class MTLIntersectionFunctionDescriptor

A description of an intersection function that performs an intersection test.

class MTLIntersectionFunctionTableDescriptor

A specification of how to create an intersection function table.

protocol MTLIntersectionFunctionTable

A table of intersection functions that Metal calls to perform ray-tracing intersection tests.

