

- SpriteKit
- SKShader
-  addUniform(\_:) 

Instance Method

# addUniform(\_:)

Adds a uniform to the shader.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func addUniform(_ uniform: SKUniform)
```

## Parameters 

`uniform`  

The new uniform object to add. The uniform object’s name must not already be in use by another uniform attached to the shader.

## Discussion

The uniform variable is automatically accessible inside your shader; do not add a declaration for it in your shader’s source code. The uniform *must* be accessed in the fragment shader.

## See Also

### Providing Uniform Data to a Shader

func removeUniformNamed(String)

Removes a uniform from the shader.

var uniforms: [SKUniform]

The list of uniforms associated with the shader.

func uniformNamed(String) -> SKUniform?

Returns the uniform object corresponding to a particular uniform variable.

