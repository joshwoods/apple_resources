

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
-  PhotogrammetrySession.Configuration.CustomDetailSpecification 

Structure

# PhotogrammetrySession.Configuration.CustomDetailSpecification

A structure for specifying various customizable options on the reconstructed model and textures.

Mac Catalyst 17.0+macOS 14.0+

``` source
struct CustomDetailSpecification
```

## Topics

### Structures

struct TextureMapOutputs

Allows specification of the set of output texture maps to be included in the output model.

### Operators

static func == (PhotogrammetrySession.Configuration.CustomDetailSpecification, PhotogrammetrySession.Configuration.CustomDetailSpecification) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init()

### Instance Properties

var maximumPolygonCount: UInt

The upper limit on polygons in the model mesh.

var maximumTextureDimension: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureDimension

The maximum dimension of the reconstructed texture maps.

var outputTextureMaps: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureMapOutputs

The set of texture maps to create in the model.

var textureFormat: PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureFormat

The data type of the texture map.

### Enumerations

enum TextureDimension

One of the discrete texture dimensions to specify the size of the model texture maps. For example, a `.twoK` dimension means the texture map size can be up to size 2048x2048.

enum TextureFormat

The output format to use for all textures.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

