

- GameplayKit
- GKScene
-  graphs 

Instance Property

# graphs

The list of pathfinding graph objects managed by the scene.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var graphs: [String : GKGraph] { get }
```

## Discussion

When you define pathfinding graphs in the Xcode SpriteKit scene editor, Xcode automatically adds them to this array.

## See Also

### Managing Pathfinding Graphs

func removeGraph(String)

Removes a pathfinding graph from the list of graphs managed by the scene.

