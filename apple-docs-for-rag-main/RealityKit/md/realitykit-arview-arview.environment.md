

- RealityKit
- ARView
-  ARView.Environment 

Structure

# ARView.Environment

A description of background, lighting, and acoustic properties for a view’s content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
struct Environment
```

## Topics

### Creating an environment

init(background: ARView.Environment.Background, lighting: ARView.Environment.ImageBasedLight, reverb: ARView.Environment.Reverb)

Creates a new environment description with the given elements.

### Setting a background

var background: ARView.Environment.Background

The background for the environment.

struct Background

Content that appears as the background of the scene.

### Lighting the environment

var lighting: ARView.Environment.ImageBasedLight

The lighting used in the environment of a particular scene.

struct ImageBasedLight

Lighting properties of an environment.

### Defining acoustic properties

var reverb: ARView.Environment.Reverb

The amount of reverb in the scene.

enum Reverb

Reverb characteristics of an environment.

### Structures

struct SceneUnderstanding

An object that holds scene-understanding options for the view.

### Instance Properties

var sceneUnderstanding: ARView.Environment.SceneUnderstanding

The scene-understanding options for the view.

### Type Aliases

typealias Color

An alias for the color type that’s appropriate for the current platform.

## See Also

### Visual environment adjustments

struct RealityViewEnvironment

A struct that determines the background and default lighting properties for a reality view.

struct RealityViewRenderingEffects

A struct for enabling and disabling rendering effects for RealityKit content.

struct RealityViewRenderingEffectMode

A mode that determines whether a rendering effect is enabled or disabled.

struct RealityViewDynamicRange

Options that determine the state of high dynamic range rendering for virtual content.

enum AntialiasingMode

The rendering technique used to smooth edges of virtual content.

struct RenderOptions

The available rendering options that you use to selectively disable certain rendering effects.

