

- RealityKit
-  ImageBasedLightComponent 

Structure

# ImageBasedLightComponent

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct ImageBasedLightComponent
```

## Topics

### Operators

static func == (ImageBasedLightComponent, ImageBasedLightComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(source: ImageBasedLightComponent.Source, intensityExponent: Float)

### Instance Properties

var inheritsRotation: Bool

Whether the IBL inherit the rotation of the Entity

var intensityExponent: Float

The intensity value of the probe An intensityExponent of 0 means using the diffuse/specular intensities as-is Otherwise the intensity is multiplied by 2^intensityExponent

var source: ImageBasedLightComponent.Source

Image(s) of the lighting environment

### Enumerations

enum Source

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Image-based lights

enum Source

struct ImageBasedLightReceiverComponent

