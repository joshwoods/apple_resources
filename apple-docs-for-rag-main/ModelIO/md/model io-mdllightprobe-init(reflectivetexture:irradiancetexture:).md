

- Model I/O
- MDLLightProbe
-  init(reflectiveTexture:irradianceTexture:) 

Initializer

# init(reflectiveTexture:irradianceTexture:)

Initializes a light probe with the specified cube map textures.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    reflectiveTexture: MDLTexture?,
    irradianceTexture: MDLTexture?
)
```

## Parameters 

`reflectiveTexture`  

A cube map texture that contains a rendering of a scene as seen from the light probe’s position.

`irradianceTexture`  

A cube map texture that contains samples of the total light arriving at the light probe’s position from every direction.

## Return Value

A new light probe object.

## Discussion

You can derive an irradiance map from a reflective texture with methods on the MDLTexture class, or when creating a light probe with the init(textureSize:forLocation:lightsToConsider:objectsToConsider:reflectiveCubemap:irradianceCubemap:) method.

