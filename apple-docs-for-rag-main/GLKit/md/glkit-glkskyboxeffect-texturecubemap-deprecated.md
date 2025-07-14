

- GLKit
- GLKSkyboxEffect
-  textureCubeMap Deprecated

Instance Property

# textureCubeMap

The texture to apply to the skybox.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var textureCubeMap: GLKEffectPropertyTexture { get }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

Your application should create a complete texture cube map in its initialization code. Then, assign the name of this texture to the textureCubeMap property of the skybox object.

```
skyboxEffect.textureCubeMap.glName = texture_name;
```

## See Also

### Configuring the Skybox

var center: GLKVector3

The center of the skybox.

Deprecated

var xSize: GLfloat

The width of the skybox.

Deprecated

var ySize: GLfloat

The height of the skybox.

Deprecated

var zSize: GLfloat

The depth of the skybox.

Deprecated

