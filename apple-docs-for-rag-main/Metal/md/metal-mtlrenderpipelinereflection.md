

- Metal
-  MTLRenderPipelineReflection 

Class

# MTLRenderPipelineReflection

Information about the arguments of a graphics function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLRenderPipelineReflection
```

## Overview

The MTLRenderPipelineReflection class is an interface that represents the parameters for the shaders in a render pipeline state (see MTLRenderPipelineState). Each pipeline state can include object, mesh, vertex, fragment, and tile shaders.

You create a reflection instance at the same time as the pipeline state that it represents by calling the appropriate MTLDevice method. For example, the makeRenderPipelineState(descriptor:options:reflection:) and makeRenderPipelineState(descriptor:options:completionHandler:) methods create the pipeline state and the reflection instances at the same time.

Important

Only create reflection instances if you need them because each one can require a significant amount of memory.

For more information, see Pipeline State Creation.

## Topics

### Inspecting a Shader’s Parameter

var fragmentBindings: [any MTLBinding]

An array of binding instances, each of which represents a parameter of the pipeline state’s fragment shader.

var meshBindings: [any MTLBinding]

An array of binding instances, each of which represents a parameter of the pipeline state’s mesh shader.

var objectBindings: [any MTLBinding]

An array of binding instances, each of which represents a parameter of the pipeline state’s object shader.

var tileBindings: [any MTLBinding]

An array of binding instances, each of which represents a parameter of the pipeline state’s tile shader.

var vertexBindings: [any MTLBinding]

An array of binding instances, each of which represents a parameter of the pipeline state’s vertex shader.

### Deprecated

var vertexArguments: [MTLArgument]?

An array of argument instances, each of which represent a parameter of the pipeline state’s vertex shader.

Deprecated

var fragmentArguments: [MTLArgument]?

An array of argument instances, each of which represent a parameter of the pipeline state’s fragment shader.

Deprecated

var tileArguments: [MTLArgument]?

An array of argument instances, each of which represent a parameter of the pipeline state’s tile shader.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Introspection Data

class MTLComputePipelineReflection

Information about the arguments of a compute function.

typealias MTLAutoreleasedComputePipelineReflection

A convenience type alias for an autoreleased compute pipeline reflection object.

typealias MTLAutoreleasedRenderPipelineReflection

A convenience type alias for an autoreleased pipeline reflection instance.

enum MTLBindingType

protocol MTLBinding

enum MTLBindingAccess

protocol MTLBufferBinding

protocol MTLTextureBinding

protocol MTLThreadgroupBinding

protocol MTLObjectPayloadBinding

