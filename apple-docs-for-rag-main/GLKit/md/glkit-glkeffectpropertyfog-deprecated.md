

- GLKit
-  GLKEffectPropertyFog Deprecated

Class

# GLKEffectPropertyFog

Fog drawing information for use in GLKit rendering effects.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
class GLKEffectPropertyFog
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Overview

These properties are specifically designed to mimic the fog calculations provided by OpenGL ES 1.1.

When fog is enabled, the fog component is calculated and clamped to a range from `0.0` to `1.0`. Then, the fog value is used as a blending factor between the computed fragment color and the fog color.

## Topics

### Enabling Fog

var enabled: GLboolean

A Boolean value that indicates whether fog is applied to the fragment color.

### Choosing the Fog Mode

var mode: GLint

The algorithm used to compute the density of the fog applied to the fragment color.

### Fog Properties

var color: GLKVector4

The color of the fog at maximum density.

var density: GLfloat

The rate at which the fog exponent increases.

var start: GLfloat

The minimum distance in eye coordinates before fog is applied to the fragment color.

var end: GLfloat

The distance in eye coordinates where fog completely covers the color fragment.

### Constants

enum GLKFogMode

A mode that describes how the fog component is calculated for the fragment.

## Relationships

### Inherits From

- GLKEffectProperty

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Rendering Effect Parameters

class GLKEffectProperty

The abstract superclass for configuration information used in GLKit rendering effects.

Deprecated

class GLKEffectPropertyLight

Lighting information for use in GLKit rendering effects.

Deprecated

class GLKEffectPropertyTexture

Texture drawing parameters for use in GLKit rendering effects.

Deprecated

class GLKEffectPropertyMaterial

Surface appearance properties for use in GLKit rendering effects.

Deprecated

class GLKEffectPropertyTransform

Coordinate transform information for use in GLKit rendering effects.

Deprecated

GLKit Effects Constants

