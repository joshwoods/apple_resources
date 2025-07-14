

- SceneKit
- SCNProgram
-  library 

Instance Property

# library

The Metal shader library containing shader functions to be used by this program.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var library: (any MTLLibrary)? { get set }
```

## Discussion

If this property’s value is nil (the default), SceneKit loads shader functions from the default Metal library. Change this value if you have compiled a separate `.metallib` file for the shader functions you wish to use.

## See Also

### Related Documentation

func makeDefaultLibrary() -> (any MTLLibrary)?

Creates a Metal library instance that contains the functions from your app’s default Metal library.

### Working With Metal Shaders

var vertexFunctionName: String?

The name of the vertex shader function to load from a Metal shader library.

var fragmentFunctionName: String?

The name of the fragment shader function to load from a Metal shader library.

