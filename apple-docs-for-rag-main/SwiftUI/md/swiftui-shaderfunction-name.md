

- SwiftUI
- ShaderFunction
-  name 

Instance Property

# name

The name of the shader function in the library.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var name: String
```

## See Also

### Configuring a function

var library: ShaderLibrary

The shader library storing the function.

func dynamicallyCall(withArguments: [Shader.Argument]) -> Shader

Returns a new shader by applying the provided argument values to the referenced function.

