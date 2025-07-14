

- RealityKit
- PhotogrammetrySession
-  PhotogrammetrySession.Configuration 

Structure

# PhotogrammetrySession.Configuration

The configuration parameters for a photogrammetry session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Configuration
```

## Mentioned in 

Creating 3D objects from photographs

## Overview

A PhotogrammetrySession.Configuration instance may be passed in to any of the PhotogrammetrySession initializers to override its default values.

Use the default values in most instances. In some cases, you may improve the quality of the generated 3D object by specifying different values. If, for example, your source images have few landmarks or poor contrast, you might set featureSensitivity to PhotogrammetrySession.Configuration.FeatureSensitivity.high to compensate for it.

## Topics

### Creating a configuration

init()

Creates a configuration using default values.

### Configuring object masking

var isObjectMaskingEnabled: Bool

A Boolean value that indicates whether the session uses object masks.

### Configuring sample ordering

var sampleOrdering: PhotogrammetrySession.Configuration.SampleOrdering

The order of the image samples.

enum SampleOrdering

The ordering of samples.

### Configuring feature sensitivity

var featureSensitivity: PhotogrammetrySession.Configuration.FeatureSensitivity

The precision of landmark detection.

enum FeatureSensitivity

The sensitivity to sample landmarks.

### Structures

struct CustomDetailSpecification

A structure for specifying various customizable options on the reconstructed model and textures.

### Operators

static func == (PhotogrammetrySession.Configuration, PhotogrammetrySession.Configuration) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(checkpointDirectory: URL)

### Instance Properties

var checkpointDirectory: URL?

The directory that a the photogrammetry session uses for checkpoints during reconstruction.

var customDetailSpecification: PhotogrammetrySession.Configuration.CustomDetailSpecification

Defines custom detail level specifications for a photogrammetry session with custom detail level.

var ignoreBoundingBox: Bool

Ignores any bounding box information embedded in the input images and instead returns all possible geometry that can be automatically estimated using the image set. The resulting mesh will likely need post-processing. Note: to recover the entire scene geometry as well as ignore the box, `isObjectMaskingEnabled` should also be set to false.

var meshPrimitive: PhotogrammetrySession.Configuration.MeshPrimitive

On macOS, this property can be used to change the output geometry mesh primitive for all output geometry in the session, regardless of `Detail` setting. This will also change the mesh primitives in both OBJ and USD outputs. By default, triangle meshes are created.

### Enumerations

enum MeshPrimitive

The type of geometric mesh primitives to create in model output

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Configuring the session

var configuration: PhotogrammetrySession.Configuration

Readonly property containing the session configuration set in the construction.

