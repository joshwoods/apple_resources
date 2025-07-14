

- SceneKit
- SCNProgram
-  fragmentFunctionName 

Instance Property

# fragmentFunctionName

The name of the fragment shader function to load from a Metal shader library.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var fragmentFunctionName: String? { get set }
```

## Discussion

A program’s fragment shader (sometimes called a *pixel shader*) executes at least once for each pixel in rendered output. The fragment shader takes as input the values output by the vertex shader (after those values have been interpolated by the GPU), and uses them to compute a final color for each pixel.

By default, SceneKit looks for a fragment shader function by this name in the default Metal library. To use shaders from a separate library file, change the library property.

## See Also

### Working With Metal Shaders

var vertexFunctionName: String?

The name of the vertex shader function to load from a Metal shader library.

var library: (any MTLLibrary)?

The Metal shader library containing shader functions to be used by this program.

