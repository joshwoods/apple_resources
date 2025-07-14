

- GameplayKit
- GKScene
-  entities 

Instance Property

# entities

The list of GameplayKit entities managed by the scene.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var entities: [GKEntity] { get }
```

## Discussion

When you add entities (and their components) to a scene in the Xcode SpriteKit scene editor, Xcode automatically adds them to this array.

## See Also

### Managing Entities and Components

func addEntity(GKEntity)

Adds a GameplayKit entity to the list of entities managed by the scene.

func removeEntity(GKEntity)

Removes a GameplayKit entity from the list of entities managed by the scene.

