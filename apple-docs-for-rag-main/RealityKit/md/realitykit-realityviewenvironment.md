

- RealityKit
-  RealityViewEnvironment 

Structure

# RealityViewEnvironment

A struct that determines the background and default lighting properties for a reality view.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct RealityViewEnvironment
```

## Topics

### Setting the environment background

static var `default`: RealityViewEnvironment

The view uses any background style you apply via the view’s background style.

static func skybox(EnvironmentResource) -> RealityViewEnvironment

The view uses a skybox environment as the background.

## Relationships

### Conforms To

- Sendable

## See Also

### Visual environment adjustments

struct RealityViewRenderingEffects

A struct for enabling and disabling rendering effects for RealityKit content.

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

