

- RealityKit
-  RealityViewRenderingEffects 

Structure

# RealityViewRenderingEffects

A struct for enabling and disabling rendering effects for RealityKit content.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct RealityViewRenderingEffects
```

## Topics

### Instance Properties

var antialiasing: AntialiasingMode

Enables or disables an antialiasing effect which smooths the edges of virtual content.

var cameraGrain: RealityViewRenderingEffectMode

Enables or disables an image noise effect for virtual content.

var depthOfField: RealityViewRenderingEffectMode

Enables or disables a depth of field effect for virtual content.

var dynamicRange: RealityViewDynamicRange

Enables or disables high dynamic range rendering for virtual content.

var motionBlur: RealityViewRenderingEffectMode

Enables or disables a motion blur effect for virtual content.

## Relationships

### Conforms To

- Sendable

## See Also

### Visual environment adjustments

struct RealityViewEnvironment

A struct that determines the background and default lighting properties for a reality view.

struct RealityViewRenderingEffectMode

A mode that determines whether a rendering effect is enabled or disabled.

struct RealityViewDynamicRange

Options that determine the state of high dynamic range rendering for virtual content.

enum AntialiasingMode

The rendering technique used to smooth edges of virtual content.

struct Environment

A description of background, lighting, and acoustic properties for a view’s content.

struct RenderOptions

The available rendering options that you use to selectively disable certain rendering effects.

