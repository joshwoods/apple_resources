

- GLKit
- GLKEffectPropertyLight
-  quadraticAttenuation Deprecated

Instance Property

# quadraticAttenuation

A quadratic factor applied to the attenuation of a point light or spotlight.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var quadraticAttenuation: GLfloat { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The distance attenuation factor is calculated as `1.0 / (k0 + k1 * d + k2 * d * d)`, where `d` represents the distance from the light to the point being lit. The quadraticAttenuation property is represented in this calculation as `k2`. The default value is `0.0`.

## See Also

### Configuring Lighting Attenuation

var constantAttenuation: GLfloat

A constant factor applied to the attenuation of a point light or spotlight.

Deprecated

var linearAttenuation: GLfloat

A linear factor applied to the attenuation of a point light or spotlight.

Deprecated

