

- SceneKit
-  SCNShadowMode 

Enumeration

# SCNShadowMode

Options for SceneKit’s rendering of shadows cast by a light, used by the shadowMode property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNShadowMode
```

## Overview

Each shadow mode may have a positive or negative effect on rendering performance, depending on the contents of the scene. Test your app to determine which shadow mode provides the best balance between performance and quality for the scenes you want to render.

## Topics

### Constants

case forward

SceneKit renders shadows during lighting computations.

case deferred

SceneKit renders shadows in a postprocessing pass.

case modulated

SceneKit renders shadows by projecting the light’s gobo image. The light does not illuminate the scene.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing Shadows Cast by the Light

var castsShadow: Bool

A Boolean value that determines whether the light casts shadows.

var shadowRadius: CGFloat

A number that specifies the amount of blurring around the edges of shadows cast by the light. Animatable.

var shadowColor: Any

The color of shadows cast by the light. Animatable.

var shadowMapSize: CGSize

The size of the shadow map image that SceneKit renders when creating shadows.

var shadowSampleCount: Int

The number of samples from the shadow map that SceneKit uses to render each pixel.

var shadowMode: SCNShadowMode

The mode SceneKit uses to render shadows.

var shadowBias: CGFloat

The amount of correction to apply to the shadow to prevent rendering artifacts.

var orthographicScale: CGFloat

The orthographic scale SceneKit uses when rendering the shadow map for a directional light.

var zFar: CGFloat

The maximum distance between the light and a visible surface for casting shadows.

var zNear: CGFloat

The minimum distance between the light and a visible surface for casting shadows. Animatable.

