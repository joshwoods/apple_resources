

- Model I/O
-  MDLObjectContainerComponent 

Protocol

# MDLObjectContainerComponent

The general interface for classes that can act as containers in an object hierarchy.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol MDLObjectContainerComponent : NSFastEnumeration, MDLComponent
```

## Overview

Model I/O uses this interface to represent content loaded from an asset file. Various asset file formats define collections of information to describe their contents, such as a hierarchy of transforms to model the spatial relationships between models, lights, and meshes contained in an asset. When Model I/O imports such asset formats, the contents of the asset are objects implementing this protocol. You can also adopt this protocol in your own classes to describe your own custom asset formats—for example, one that includes collections of scripts and their triggers associated with the objects in a scene.

## Topics

### Working with Child Objects

var objects: [MDLObject]

This object’s array of child objects.

**Required**

func add(MDLObject)

Adds the specified object as a child of this object.

**Required**

func remove(MDLObject)

Removes the specified object from this object’s array of children.

**Required**

### Instance Properties

var count: Int

**Required**

### Subscripts

subscript(Int) -> MDLObject

**Required**

## Relationships

### Inherits From

- MDLComponent
- NSFastEnumeration
- NSObjectProtocol

### Conforming Types

- MDLObjectContainer

## See Also

### Extensible Asset Format Support

protocol MDLComponent

The base protocol for extensible file format support in Model I/O.

class MDLObjectContainer

A default implementation for handling object hierarchy relationships in a 3D asset.

protocol MDLTransformComponent

The general interface for classes that manage local coordinate space transforms for 3D objects

