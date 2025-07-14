

- GLKit
- GLKBaseEffect
-  lightModelTwoSided Deprecated

Instance Property

# lightModelTwoSided

A Boolean value that indicates whether lighting is calculated for both sides of a primitive.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var lightModelTwoSided: GLboolean { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

If the value is `GL_TRUE` and the back face of a primitive is being rendered, the lighting values are calculated by negating the surface normals for the primitive. If the value is `GL_FALSE`, then the facing of the primitive is ignored when performing the lighting calculation. The default value is `GL_FALSE`.

Setting the value of this property to `GL_TRUE` may impact performance. Only use two-sided lighting when either side of a primitive could theoretically be visible to the camera.

## See Also

### Configuring Lights

var lightingType: GLKLightingType

The strategy the effect uses to calculate light values at each fragment. See GLKLightingType.

Deprecated

var material: GLKEffectPropertyMaterial

The material properties used when calculating the light values for a rendered primitive.

Deprecated

var lightModelAmbientColor: GLKVector4

The ambient color applied to all primitives rendered by the effect.

Deprecated

var light0: GLKEffectPropertyLight

The lighting properties for the first light in the scene.

Deprecated

var light1: GLKEffectPropertyLight

The lighting properties for the second light in the scene.

Deprecated

var light2: GLKEffectPropertyLight

The lighting properties for the third light in the scene.

Deprecated

