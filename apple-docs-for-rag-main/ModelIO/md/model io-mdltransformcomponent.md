

- Model I/O
-  MDLTransformComponent 

Protocol

# MDLTransformComponent

The general interface for classes that manage local coordinate space transforms for 3D objects

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol MDLTransformComponent : MDLComponent
```

## Overview

Transform information—that is, the combination of an object’s position, orientation, shear, and scale—can be static, or in the case of resources that describe animations, time-based. By default, the MDLTransform class manages transform information for objects loaded from a MDLAsset instance. By providing your own class that adopts this protocol, you can support other ways to associate transform information with objects—for example, when defining a custom asset file format.

## Topics

### Working with Static Transforms

var matrix: matrix_float4x4

The transform matrix that defines the local coordinate space relative to a parent coordinate space.

**Required**

func setLocalTransform(matrix_float4x4)

Sets a new static transform matrix, overriding any time-based transform information.

### Working with Animated Transforms

var minimumTime: TimeInterval

The timestamp for the first timed data sample in the transform component.

**Required**

var maximumTime: TimeInterval

The timestamp for the last timed data sample in the transform component.

**Required**

func localTransform(atTime: TimeInterval) -> matrix_float4x4

Returns the local transform matrix as of the specified time sample.

func setLocalTransform(matrix_float4x4, forTime: TimeInterval)

Sets a new local transform matrix for the specified time sample.

### Deriving a Global Transformation

static func globalTransform(with: MDLObject, atTime: TimeInterval) -> matrix_float4x4

Returns the absolute coordinate transformation for an object in a transform hierarchy.

### Instance Properties

var keyTimes: [NSNumber]

**Required**

var resetsTransform: Bool

**Required**

## Relationships

### Inherits From

- MDLComponent
- NSObjectProtocol

### Conforming Types

- MDLTransform
- MDLTransformStack

## See Also

### Extensible Asset Format Support

protocol MDLComponent

The base protocol for extensible file format support in Model I/O.

class MDLObjectContainer

A default implementation for handling object hierarchy relationships in a 3D asset.

protocol MDLObjectContainerComponent

The general interface for classes that can act as containers in an object hierarchy.

