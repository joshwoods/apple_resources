

- SwiftUI
- ShaderFunction
-  library 

Instance Property

# library

The shader library storing the function.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var library: ShaderLibrary
```

## See Also

### Configuring a function

var name: String

The name of the shader function in the library.

func dynamicallyCall(withArguments: [Shader.Argument]) -> Shader

Returns a new shader by applying the provided argument values to the referenced function.

