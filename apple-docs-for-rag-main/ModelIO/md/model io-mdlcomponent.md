

- Model I/O
-  MDLComponent 

Protocol

# MDLComponent

The base protocol for extensible file format support in Model I/O.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol MDLComponent : NSObjectProtocol
```

## Overview

By extending this protocol in your own custom protocols, you can define new functionality to add to the MDLObject instances in the object graph corresponding to a MDLAsset instance.

Model I/O adopts this pattern to support container objects (with the MDLObjectContainerComponent protocol) and objects with associated transformations (with the MDLTransformComponent protocol). To work with these aspects of a Model I/O object, call the object’s componentConforming(to:) method with the appropriate protocol. (The MDLObject class also provides convenience methods and properties for accessing features of these components without directly accessing the component instances.)

To add your own object features, first define a protocol that extends the MDLComponent protocol, implement a class that adopts that protocol, and then use the setComponent(_:for:) method to add your component to each object that needs it. The example below shows how you might implement a file format that associates scripting event triggers with parts of a game scene.

```
```

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MDLObjectContainerComponent
- MDLTransformComponent

### Conforming Types

- MDLAnimationBindComponent
- MDLObjectContainer
- MDLTransform
- MDLTransformStack

## See Also

### Extensible Asset Format Support

class MDLObjectContainer

A default implementation for handling object hierarchy relationships in a 3D asset.

protocol MDLObjectContainerComponent

The general interface for classes that can act as containers in an object hierarchy.

protocol MDLTransformComponent

The general interface for classes that manage local coordinate space transforms for 3D objects

