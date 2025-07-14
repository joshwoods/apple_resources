

- RealityKit
- ModelDebugOptionsComponent
-  ModelDebugOptionsComponent.VisualizationMode 

Enumeration

# ModelDebugOptionsComponent.VisualizationMode

A mode that specifies the portion of the rendering process to isolate and display for debugging.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
enum VisualizationMode
```

## Topics

### Visualization modes

case none

A mode that doesn’t display a visualization.

case normal

A mode that displays the normal vectors as a color.

case tangent

A mode that displays the surface tangent vectors as a color.

case bitangent

A mode that displays the surface bitangent vectors as a color.

case baseColor

A mode that displays the entity’s base color with no lighting or material properties applied.

case textureCoordinates

A mode that displays the texture coordinates as a color.

case finalColor

A mode that displays the entity’s calculated color, ignoring transparency.

case finalAlpha

A mode that displays the entity’s calculated transparency as its surface color.

case roughness

A mode that displays the shininess of a material as the surface color.

case metallic

A mode that displays the reflectiveness of an entity as its surface color.

case ambientOcclusion

A mode that displays the calculated ambient occlusion value as the surface color.

case specular

A mode that displays en entity’s shininess as its surface color.

case emissive

A mode that displays the emissive channel of a material as the surface color.

case clearcoat

A mode that displays the clearcoat channel of a material as the surface color.

case clearcoatRoughness

A mode that displays the clearcoat roughness channel of a material as the surface color.

case lightingDiffuse

A mode that displays the intensity of indirect light hitting the entity as its surface color.

case lightingSpecular

A mode that displays the intensity of direct light hitting the entity as its surface color.

### Raw values

init?(rawValue: String)

Creates a new instance with the specified raw value.

var rawValue: String

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Comparators

var hashValue: Int

func hash(into: inout Hasher)

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Enumeration Cases

case clearcoatNormal

A mode that displays the clearcoat normal of a material as the surface color.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Setting the visualization mode

var visualizationMode: ModelDebugOptionsComponent.VisualizationMode

The part of the rendering process to display as the entity’s surface texture.

