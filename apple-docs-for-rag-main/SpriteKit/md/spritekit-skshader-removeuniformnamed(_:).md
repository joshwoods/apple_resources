

- SpriteKit
- SKShader
-  removeUniformNamed(\_:) 

Instance Method

# removeUniformNamed(\_:)

Removes a uniform from the shader.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func removeUniformNamed(_ name: String)
```

## Parameters 

`name`  

The name of the uniform to remove.

## Discussion

If a uniform with that name does not exist in the shader, nothing happens.

## See Also

### Providing Uniform Data to a Shader

func addUniform(SKUniform)

Adds a uniform to the shader.

var uniforms: [SKUniform]

The list of uniforms associated with the shader.

func uniformNamed(String) -> SKUniform?

Returns the uniform object corresponding to a particular uniform variable.

