

- Model I/O
-  MDLObject 

Class

# MDLObject

The base class for objects that are part of a 3D asset, including meshes, cameras, and lights.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class MDLObject
```

## Overview

When you load content from an asset file using the MDLAsset class, Model I/O creates instances of the MDLObject subclasses MDLMesh, MDLCamera, and MDLLight. For asset formats that describe a collection of meshes, cameras, and lights organized in a hierarchy of spatial transforms, Model I/O also creates instances of the MDLObject class itself to describe the transform nodes that organize the asset’s visual content. Similarly, you use the MDLObject class and its subclasses when creating an object graph to be exported as an asset file using the MDLAsset class.

### Extending Model I/O with Components

Model I/O allows you to customize the content and relationships in an object graph with *components*. For each aspect of an object’s functionality, you use a component protocol (extending the MDLComponent protocol) to define functionality and a class adopting that protocol to implement it. Then, you can use the componentConforming(to:) and setComponent(_:for:) methods to associate those objects with any instance of the MDLObject class or of one of its subclasses. For example, you might define a protocol to add gameplay-related information such as scripting triggers to certain meshes, lights, or cameras in a scene.

Model I/O itself uses this mechanism to handle object hierarchies and spatial transforms: The methods listed in Working with Object Hierarchies use the MDLObjectContainerComponent protocol to model hierarchic relationships between objects in an asset, and the methods listed in Working with Objects in Space use the MDLTransformComponent protocol to model coordinate space relationships. To add support for an asset file format or object graph that uses other ways to store or compute these relationships, you can use your own classes that adopt these protocols.

## Topics

### Customizing Objects with Components

func componentConforming(to: Protocol) -> (any MDLComponent)?

Returns the object’s component for the specified protocol.

func setComponent(any MDLComponent, for: Protocol)

Associates a component with the object for the specified protocol.

### Working with Object Hierarchies

var parent: MDLObject?

The parent object that contains this object.

var children: any MDLObjectContainerComponent

A component that manages this object’s collection of children.

func addChild(MDLObject)

Adds a child object to this object, creating a container for the object’s children if necessary.

func enumerateChildObjects(of: AnyClass, root: MDLObject, using: (MDLObject, UnsafeMutablePointer&lt;ObjCBool>) -> Void, stopPointer: UnsafeMutablePointer&lt;ObjCBool>)

Executes the specified block using each object in this object’s child hierarchy.

var path: String

A path that identifies the object in an asset’s object hierarchy using object names.

func atPath(String) -> MDLObject

Returns the child object at the specified path.

### Working with Objects in Space

func boundingBox(atTime: TimeInterval) -> MDLAxisAlignedBoundingBox

Returns the minimum region entirely enclosing the object’s contents at the specified time sample.

var transform: (any MDLTransformComponent)?

A component that manages this object’s spatial transform and its changes over time.

### Managing Rendering Intent

var hidden: Bool

A Boolean value indicating whether this object should be used in rendering.

var instance: MDLObject?

The primary object, if applicable, of which this object is an instance.

var path: String

A path that identifies the object in an asset’s object hierarchy using object names.

var components: [any MDLComponent]

### Object Instancing

func atPath(String) -> MDLObject

Returns the child object at the specified path.

func enumerateChildObjects(of: AnyClass, root: MDLObject, using: (MDLObject, UnsafeMutablePointer&lt;ObjCBool>) -> Void, stopPointer: UnsafeMutablePointer&lt;ObjCBool>)

Executes the specified block using each object in this object’s child hierarchy.

subscript(Protocol) -> (any MDLComponent)?

### Constants

struct MDLAxisAlignedBoundingBox

The minimal volume containing an object, used by the boundingBox(atTime:) method.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MDLCamera
- MDLLight
- MDLMesh
- MDLPackedJointAnimation
- MDLSkeleton
- MDLVoxelArray

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLNamed
- NSObjectProtocol

## See Also

### 3D Asset Basics

class MDLAsset

An indexed container for 3D objects and associated information, such as transform hierarchies, meshes, cameras, and lights.

class MDLTransform

A description of the local coordinate space transformations for a 3D object.

class MDLMesh

A container for vertex buffer data to be used in rendering a 3D object.

class MDLSubmesh

A container for index buffer data and material information to be used in rendering all or part of a 3D object.

class MDLSubmeshTopology

A description of how a submesh’s index buffer data is arranged and how that arrangement should be used to produce the submesh’s intended 3D shape.

protocol MDLNamed

The common interface for Model I/O objects that expose a human-readable name.

