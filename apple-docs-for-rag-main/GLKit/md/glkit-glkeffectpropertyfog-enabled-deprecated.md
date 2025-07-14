

- GLKit
- GLKEffectPropertyFog
-  enabled Deprecated

Instance Property

# enabled

A Boolean value that indicates whether fog is applied to the fragment color.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var enabled: GLboolean { get set }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

If the value of this property is `GL_TRUE`, then fog calculations are performed each time a fragment is computed. If the value of this property is `GL_FALSE`, then fog calculations are skipped. The default value is `GL_TRUE`.

