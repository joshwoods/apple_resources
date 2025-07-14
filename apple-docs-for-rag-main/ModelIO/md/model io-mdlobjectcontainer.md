

- Model I/O
-  MDLObjectContainer 

Class

# MDLObjectContainer

A default implementation for handling object hierarchy relationships in a 3D asset.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLObjectContainer
```

## Overview

Model I/O uses the MDLObjectContainerComponent protocol to create object hierarchy relationships for meshes, lights, cameras, and containers loaded from a MDLAsset instance. To create your own containers—for example, to reference in-memory representations, offline databases, or custom asset file formats—create MDLObjectContainer subclasses and add them to a MDLObject instance using its setComponent(_:for:) method.

All methods of this class are defined by the MDLObjectContainerComponent protocol. For discussion of these methods, see MDLObjectContainerComponent.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLComponent
- MDLObjectContainerComponent
- NSFastEnumeration
- NSObjectProtocol

## See Also

### Extensible Asset Format Support

protocol MDLComponent

The base protocol for extensible file format support in Model I/O.

protocol MDLObjectContainerComponent

The general interface for classes that can act as containers in an object hierarchy.

protocol MDLTransformComponent

The general interface for classes that manage local coordinate space transforms for 3D objects

