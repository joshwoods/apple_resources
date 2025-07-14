

- GameplayKit
-  GKScene 

Class

# GKScene

A container for associating GameplayKit objects with a SpriteKit scene.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class GKScene
```

## Overview

When you create a scene in the Xcode SpriteKit scene editor, Xcode automatically creates a GKScene object to manage any GameplayKit objects you add to the scene (entities, components, or pathfinding graphs) and archive them alongside the SpriteKit scene content.

To use a SpriteKit scene that contains GameplayKit objects, load the scene file with the GKScene init(fileNamed:) method. You can then use the entities and graphs properties to access the GKEntity (and associated GKComponent) objects and GKGraph objects in the scene, and the rootNode property to access the scene’s SpriteKit content.

Note

Any SpriteKit node in the scene to which you’ve attached an entity or components automatically has a GKSKNodeComponent object to manage the relationship between the node and the the GKEntity object it represents.

For more information on Entity-Component architecture and pathfinding graphs, see Entities and Components and Pathfinding in GameplayKit Programming Guide.

## Topics

### Loading a Scene File

convenience init?(fileNamed: String)

Loads the specified SpriteKit scene file, creating a GKScene object containing the SpriteKit scene and associated GameplayKit objects.

### Accessing the SpriteKit Scene

var rootNode: (any GKSceneRootNodeType)?

The SpriteKit scene managed by this GKScene object.

### Managing Entities and Components

var entities: [GKEntity]

The list of GameplayKit entities managed by the scene.

func addEntity(GKEntity)

Adds a GameplayKit entity to the list of entities managed by the scene.

func removeEntity(GKEntity)

Removes a GameplayKit entity from the list of entities managed by the scene.

### Managing Pathfinding Graphs

var graphs: [String : GKGraph]

The list of pathfinding graph objects managed by the scene.

func removeGraph(String)

Removes a pathfinding graph from the list of graphs managed by the scene.

### Initializers

convenience init?(fileNamed: String, rootNode: any GKSceneRootNodeType)

### Instance Methods

func addGraph(GKGraph, name: String)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Xcode and SpriteKit Integration

protocol GKSceneRootNodeType

Identifies scene classes from other frameworks that support embedded GameplayKit information.

class GKSKNodeComponent

A component that manages a SpriteKit node.

