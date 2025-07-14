

- SceneKit
- SCNProgram
-  vertexFunctionName 

Instance Property

# vertexFunctionName

The name of the vertex shader function to load from a Metal shader library.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var vertexFunctionName: String? { get set }
```

## Discussion

A program’s vertex shader executes once for each vertex in the geometry it renders. It takes as input the attributes of each vertex (such as position in model space, normal vectors, and texture coordinates). The vertex shader then outputs a clip-space position for the vertex, as well as values that the GPU interpolates across a surface and sends to the fragment shader.

By default, SceneKit looks for a fragment shader function by this name in the default Metal library. To use shaders from a separate library file, change the library property.

## See Also

### Working With Metal Shaders

var fragmentFunctionName: String?

The name of the fragment shader function to load from a Metal shader library.

var library: (any MTLLibrary)?

The Metal shader library containing shader functions to be used by this program.

