

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
- PhotogrammetrySession.Configuration.CustomDetailSpecification
-  PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureFormat 

Enumeration

# PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureFormat

The output format to use for all textures.

Mac Catalyst 17.0+macOS 14.0+

``` source
enum TextureFormat
```

## Topics

### Operators

static func == (PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureFormat, PhotogrammetrySession.Configuration.CustomDetailSpecification.TextureFormat) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case jpeg(compressionQuality: Float)

Textures will be output in JPG format with the given `compressionQuality` in the range of \[0, 1\], where 1.0 is highest quality (least compression, larger size) and 0.0 is the lowest quality (most compression, smallest size).

case png

Textures will be output in (uncompressed) PNG format.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

