

- GLKit
-  GLKit Effects Constants 

API Collection

# GLKit Effects Constants

## Overview

GLKit effects implement shaders to perform their calculations. These shaders require vertex data to be provided by your application. All of the effects provided by GLKit use a consistent set of indices to reference vertex data provided by your application. When your application enables a vertex attribute array by calling the `glEnableVertexAttribArray` function, or specifies the vertex attribute pointer by calling the `glVertexAttribPointer` function, it uses one of these constants to specify the `index` parameter.

## Topics

### Constants

enum GLKVertexAttrib

Values used as indices in OpenGL code to associate vertex data with an attribute in a named shader effect.

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

class GLKEffectPropertyTransform

Coordinate transform information for use in GLKit rendering effects.

Deprecated

