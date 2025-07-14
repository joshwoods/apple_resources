

- SceneKit
- SceneView
-  SceneView.Options 

Structure

# SceneView.Options

SceneKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct Options
```

## Topics

### Type Properties

static let allowsCameraControl: SceneView.Options

static let autoenablesDefaultLighting: SceneView.Options

static let jitteringEnabled: SceneView.Options

static let rendersContinuously: SceneView.Options

static let temporalAntialiasingEnabled: SceneView.Options

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Creating a Scene View

init(scene: SCNScene?, pointOfView: SCNNode?, options: SceneView.Options, preferredFramesPerSecond: Int, antialiasingMode: SCNAntialiasingMode, delegate: (any SCNSceneRendererDelegate)?, technique: SCNTechnique?)

