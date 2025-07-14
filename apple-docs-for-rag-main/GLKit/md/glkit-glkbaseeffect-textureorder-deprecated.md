

- GLKit
- GLKBaseEffect
-  textureOrder Deprecated

Instance Property

# textureOrder

The order in which textures are applied to rendered primitives.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var textureOrder: [GLKEffectPropertyTexture]? { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The value of this property should be an array whose contents are all GLKEffectPropertyTexture objects provided by the effect. The order of these objects in the array determines the order in which the textures are applied in the shader. For example, to reverse the order that the textures are applied to a scene, your application would use the following code:

```
```

The default value is an array that executes the texture stages in increasing order, skipping any texture stages that are not enabled.

## See Also

### Configuring Textures

var texture2d0: GLKEffectPropertyTexture

The properties for the first texture.

Deprecated

var texture2d1: GLKEffectPropertyTexture

The properties for the second texture.

Deprecated

