

- GLKit
-  GLKEffectPropertyTexture Deprecated

Class

# GLKEffectPropertyTexture

Texture drawing parameters for use in GLKit rendering effects.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
class GLKEffectPropertyTexture
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Overview

The GLKEffectPropertyTexture class defines properties that are used to configure an OpenGL texturing operation. The texturing operation combines an input color and a color sampled from the texture and outputs a new color to the next stage of calculations. The envMode property determines the function used to calculate the output color from the two input colors.

If an effect only includes a single texture property, then the input color is the lighting color calculated by the lighting stage of the graphics pipeline. An effect can also include multiple GLKEffectPropertyTexture objects. When an effect includes multiple properties, the first texture stage uses the lighting color as the first input color. Each texture stage after that uses the output of the previous stage as the input color.

## Topics

### Configuring Texture Properties

var enabled: GLboolean

A Boolean value that indicates whether this texture is used to texture drawn primitives.

var envMode: GLKTextureEnvMode

The mode the texture uses to compute its output fragment color. See GLKTextureEnvMode.

var name: GLuint

The OpenGL name for the texture being sampled by this texture stage.

var target: GLKTextureTarget

The kind of texture pointed to by the texture stage. See GLKTextureTarget.

### Constants

enum GLKTextureTarget

The kind of texture pointed to by the property.

enum GLKTextureEnvMode

The mode used to combine the texture with other color components.

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

class GLKEffectPropertyMaterial

Surface appearance properties for use in GLKit rendering effects.

Deprecated

class GLKEffectPropertyTransform

Coordinate transform information for use in GLKit rendering effects.

Deprecated

GLKit Effects Constants

