

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
-  PhotogrammetrySession.Request.Detail 

Enumeration

# PhotogrammetrySession.Request.Detail

Supported levels of detail for a request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum Detail
```

## Overview

On iOS, only one detail level – `.reduced` – is currently supported. This level is optimized for generation and viewing entirely on mobile devices.

On macOS, RealityKit object creation can generate models at different levels of detail. Higher levels of detail may take longer to create, require more memory and processing power to generate, and create objects with more complex geometry and texture requirements.

### Set a Level of Complexity

Each detail level corresponds to an object of a specific size and complexity. Here’s the expected final size of the generated object from each detail level.

| Detail Level | Triangles | Estimated File Size |
|--------------|-----------|---------------------|
| `.preview`   | \

### Create Texture Maps

Each detail level produces a 3D object with texture maps. The higher the complexity level, the larger the generated texture maps, and the more memory the system requires to display those objects in an AR scene.

RealityKit creates five texture maps at the `.full` detail level: a single diffuse map, normal map, ambient occlusion map, roughness map, and displacement map. For `.preview`, `.reduced`, and `.medium` detail levels, it produces just the single diffuse, normal and ambient occlusion maps.

When producing a model at the `.raw` detail level, only diffuse texture maps are created, but RealityKit may create up to 16 diffuse maps, each covering different parts of the model. Raw models are produced at the highest resolution possible from the source images, so they don’t benefit from having the other types of texture maps, which are used to supplement a low-resolution model with data from a higher-resolution version of the same model.

Raw models aren’t suitable for use in an AR scene and you should only use this setting if you plan to export the model to a 3D software package.

Custom detail level can be used to specify several parameters of the output mesh and textures to provide more control over the produced assets than the preset levels.

Here are the texture map sizes generated for each detail level and the amount of texture memory the uncompressed textures use at runtime.

| Detail Level | Texture Size           | Texture Memory Required |
|--------------|------------------------|-------------------------|
| `.preview`   | 1024 x 1024            | 10.666667 MB            |
| `.reduced`   | 2048 x 2048            | 42.666667 MB            |
| `.medium`    | 4096 x 4096            | 170.666667 MB           |
| `.full`      | 8192 x 8192            | 853.33333 MB            |
| `.raw`       | 8192 x 8192 (multiple) | Varies                  |
| `.custom`    | Varies                 | Varies                  |

## Topics

### Specifying a level of detail

case preview

A fast, low-quality object for previewing the final result.

case reduced

A mobile-quality object with low resource requirements.

case medium

A medium-quality object with moderate resource requirements.

case full

A high-quality object with significant resource requirements.

case raw

The raw-created object at the highest possible resolution.

### Using enumeration raw values

var rawValue: Int

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Comparing values

var hashValue: Int

func hash(into: inout Hasher)

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Enumeration Cases

case custom

A custom quality for the model, with specifics defined by the photogrammetry session.

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

### Specifying the output

case modelFile(url: URL, detail: PhotogrammetrySession.Request.Detail, geometry: PhotogrammetrySession.Request.Geometry?)

An object-creation request saved to a USDZ file or a folder (for OBJ output).

case modelEntity(detail: PhotogrammetrySession.Request.Detail, geometry: PhotogrammetrySession.Request.Geometry?)

An object-creation request stored in-memory for immediate display.

case bounds

An object-creation request that returns a box the same size as the created model.

