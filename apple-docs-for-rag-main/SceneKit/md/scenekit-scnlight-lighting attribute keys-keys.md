

- SceneKit
- SCNLight
-  Lighting Attribute Keys 

API Collection

# Lighting Attribute Keys

Keys for specifying the behavior of a light using the attribute(forKey:) and setAttribute(_:forKey:) methods.

## Overview

You can also get, set, or animate changes to the values of lighting attributes using Key-value coding with the keys listed above.

You provide or retrieve a value for each key as an NSNumber object containing the appropriate numeric type.

## Topics

### Constants

let SCNLightAttenuationStartKey: String

The distance from the light at which its intensity begins to diminish.

Deprecated

let SCNLightAttenuationEndKey: String

The distance from the light at which its intensity is completely diminished.

Deprecated

let SCNLightAttenuationFalloffExponentKey: String

The transition curve for the light’s intensity between its attenuation start and end distances.

Deprecated

let SCNLightSpotInnerAngleKey: String

The angle, in degrees, of the area fully lit by a spotlight.

Deprecated

let SCNLightSpotOuterAngleKey: String

The angle, in degrees, of the area partially lit by a spotlight.

Deprecated

let SCNLightShadowFarClippingKey: String

The maximum distance between the light and a visible surface for casting shadows.

Deprecated

let SCNLightShadowNearClippingKey: String

The minimum distance between the light and a visible surface for casting shadows.

Deprecated

## See Also

### Managing Light Attributes

var name: String?

A name associated with the light.

func attribute(forKey: String) -> Any?

Returns the value of a lighting attribute.

Deprecated

func setAttribute(Any?, forKey: String)

Sets the value for a lighting attribute.

Deprecated

