

- SpriteKit
- SKShader
-  uniforms 

Instance Property

# uniforms

The list of uniforms associated with the shader.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var uniforms: [SKUniform] { get set }
```

## Mentioned in 

Creating a Custom Fragment Shader

## Discussion

This property is not read-only, so you can also use it to provide all of the uniforms in a single operation. Each of the uniforms should be uniquely named.

## See Also

### Providing Uniform Data to a Shader

func addUniform(SKUniform)

Adds a uniform to the shader.

func removeUniformNamed(String)

Removes a uniform from the shader.

func uniformNamed(String) -> SKUniform?

Returns the uniform object corresponding to a particular uniform variable.

