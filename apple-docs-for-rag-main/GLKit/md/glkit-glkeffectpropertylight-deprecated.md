

- GLKit
-  GLKEffectPropertyLight Deprecated

Class

# GLKEffectPropertyLight

Lighting information for use in GLKit rendering effects.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
class GLKEffectPropertyLight
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Overview

The lighting model implemented by GLKEffectPropertyLight is identical to the lighting model implemented in OpenGL ES 1.1; each light interacts with any material properties on the effect to determine the intensity and color that particular light contributes to the scene at a fragment.

There are three basic kinds of lights: directional, point and spotlights.

- A directional light is considered to be infinitely far away, and always directs light in the same direction. To create a directional light, set the position property to a vector whose `x`, `y`, and `z` components specify the direction to the light (that is, the negation of the direction the light is travelling in), and whose `w` component is set to `0.0`.

- A point light is placed at a position within the scene, and emits light in all directions. To create a directional light, set the position property to a vector whose `x`, `y`, `z` and `w` components specify the homogenous coordinates for the position of the light in the scene. The `w` component is typically set to `1.0` and must not be set to `0.0`.

The intensity of a point light is adjusted using an distance attenuation function. This function is controlled by adjusting the constantAttenuation, linearAttenuation or quadraticAttenuation properties. The default values for these properties create a light whose intensity is constant over distance.

- A spotlight is placed at a position within the scene, and emits light in a specific direction in a cone. To create a spotlight, set the position property to a vector whose `x`, `y`, `z` and `w` components specify the homogenous coordinates for the position of the light in the scene. The `w` component must not be set to `0.0`. Then, set the spotDirection property to a vector that specifies the direction of the light and the spotCutoff to a value less than `180.0`.

Like a point light, a spotlight’s intensity can be adjusted using the distance attenuation properties. A spotlight’s intensity can also be changed as a function of the spotlight angle by setting the spotExponent property. The default value for a spotlight creates a spotlight whose intensity is not affected by the angle. That is, the spotlight radiates the same amount of light at the center and at the edge of the cone.

Lighting calculations are performed in eye-space coordinates.  The eye-space coordinates for the position and the spot direction are calculated at the precise moment that new position values are specified and may be affected by other properties of the effect. For more information, see GLKBaseEffect.

## Topics

### Configuring Common Lighting Properties

var enabled: GLboolean

A Boolean value that indicates whether calculations should be performed on this light.

var position: GLKVector4

The position of the light in world coordinates.

var transform: GLKEffectPropertyTransform

A transform applied to the light’s position and direction before calculating the contribution of the light.

### Configuring Light Colors

var ambientColor: GLKVector4

The ambient portion of the light.

var diffuseColor: GLKVector4

The diffuse portion of the light.

var specularColor: GLKVector4

The specular portion of the light.

### Configuring Lighting Attenuation

var constantAttenuation: GLfloat

A constant factor applied to the attenuation of a point light or spotlight.

var linearAttenuation: GLfloat

A linear factor applied to the attenuation of a point light or spotlight.

var quadraticAttenuation: GLfloat

A quadratic factor applied to the attenuation of a point light or spotlight.

### Configuring Spotlight Properties

var spotCutoff: GLfloat

The angle in degrees where the spotlight is cut off.

var spotDirection: GLKVector3

A vector indicating the direction the spotlight is projecting.

var spotExponent: GLfloat

A value indicating how focused the spotlight is.

### Constants

enum GLKLightingType

A constant that describes how lighting is calculated by an effect.

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

