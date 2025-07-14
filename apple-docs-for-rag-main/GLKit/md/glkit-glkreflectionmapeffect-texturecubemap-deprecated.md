

- GLKit
- GLKReflectionMapEffect
-  textureCubeMap Deprecated

Instance Property

# textureCubeMap

The texture map to apply in the reflection stage.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var textureCubeMap: GLKEffectPropertyTexture { get }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

Your application should create a complete texture cube map in its initialization code. Then, assign the name of this texture to the textureCubeMap property.

```
reflectionMapObject.textureCubeMap.glName = texture_name;
```

## See Also

### Effect Properties

var matrix: GLKMatrix3

The reflection matrix to apply to the normals of the submitted vertices.

Deprecated

