

- Model I/O
- MDLLightProbe
-  reflectiveTexture 

Instance Property

# reflectiveTexture

A cube map texture that contains a rendering of a scene as seen from the light probe’s position.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var reflectiveTexture: MDLTexture? { get }
```

## Discussion

A reflective texture is also known as an *environment map*. A renderer can use this texture to create reflections and specular highlights on surfaces with metallic materials.

## See Also

### Working with Textures

var irradianceTexture: MDLTexture?

A cube map texture that contains samples of the total light arriving at the light probe’s position from every direction.

