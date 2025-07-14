

- SwiftUI
- ShaderFunction
-  dynamicallyCall(withArguments:) 

Instance Method

# dynamicallyCall(withArguments:)

Returns a new shader by applying the provided argument values to the referenced function.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func dynamicallyCall(withArguments args: [Shader.Argument]) -> Shader
```

## Discussion

Typically this subscript is used implicitly via function-call syntax, for example:

let shader = ShaderLibrary.default.myFunction(.float(42))

which creates a shader passing the value `42` to the first unbound parameter of `myFunction()`.

## See Also

### Configuring a function

var library: ShaderLibrary

The shader library storing the function.

var name: String

The name of the shader function in the library.

