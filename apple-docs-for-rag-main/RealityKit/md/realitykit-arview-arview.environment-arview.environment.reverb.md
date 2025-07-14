

- RealityKit
- ARView
- ARView.Environment
-  ARView.Environment.Reverb 

Enumeration

# ARView.Environment.Reverb

Reverb characteristics of an environment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
enum Reverb
```

## Topics

### Available reverb settings

case noReverb

Omit reverb from the scene.

case preset(ARView.Environment.Reverb.Preset)

Generate reverb from a preset.

### Reverb presets

static var automatic: ARView.Environment.Reverb

The default reverb preset.

enum Preset

Available reverb preset values.

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Defining acoustic properties

var reverb: ARView.Environment.Reverb

The amount of reverb in the scene.

