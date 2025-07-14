

- GLKit
-  GLKEffectPropertyTransform Deprecated

Class

# GLKEffectPropertyTransform

Coordinate transform information for use in GLKit rendering effects.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
class GLKEffectPropertyTransform
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Overview

The GLKEffectPropertyTransform class defines properties that provide the coordinate transformations to be performed when rendering the effect.

## Topics

### Configuring Modelview Properties

var modelviewMatrix: GLKMatrix4

The matrix used to transform position coordinates from world space to eye space.

var normalMatrix: GLKMatrix3

The matrix used to transform normal coordinates from world space to eye space.

### Configuring the Projection Matrix

var projectionMatrix: GLKMatrix4

The matrix used to transform position coordinates from eye space to projection space.

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

class GLKEffectPropertyFog

Fog drawing information for use in GLKit rendering effects.

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

GLKit Effects Constants

