

- Model I/O
- MDLPhotometricLight
-  generateCubemap(fromLight:) 

Instance Method

# generateCubemap(fromLight:)

Generates a cube map texture from the light’s photometry data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func generateCubemap(fromLight textureSize: Int)
```

## Parameters 

`textureSize`  

The size (side length in pixels) of cube map texture to generate.

## Discussion

After generating a texture, use the lightCubeMap property to access it. In this texture, each texel represents the light’s intensity in the direction from the cube’s center to the texel’s position on the cube.

## See Also

### Interpreting the Light Web as a Cube Texture

var lightCubeMap: MDLTexture?

A cube map texture describing the light’s intensity in all directions.

