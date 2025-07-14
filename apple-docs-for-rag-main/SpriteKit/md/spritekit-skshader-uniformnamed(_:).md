

- SpriteKit
- SKShader
-  uniformNamed(\_:) 

Instance Method

# uniformNamed(\_:)

Returns the uniform object corresponding to a particular uniform variable.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func uniformNamed(_ name: String) -> SKUniform?
```

## Parameters 

`name`  

The name of the uniform to search for.

## Return Value

The uniform object corresponding to the name, or `nil` if that uniform cannot be found.

## See Also

### Providing Uniform Data to a Shader

func addUniform(SKUniform)

Adds a uniform to the shader.

func removeUniformNamed(String)

Removes a uniform from the shader.

var uniforms: [SKUniform]

The list of uniforms associated with the shader.

