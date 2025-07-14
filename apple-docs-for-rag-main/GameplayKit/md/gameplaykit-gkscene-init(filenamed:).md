

- GameplayKit
- GKScene
-  init(fileNamed:) 

Initializer

# init(fileNamed:)

Loads the specified SpriteKit scene file, creating a GKScene object containing the SpriteKit scene and associated GameplayKit objects.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
convenience init?(fileNamed filename: String)
```

## Parameters 

`filename`  

The name of a scene file in your app’s main bundle.

## Return Value

A new GameplayKit scene.

## Discussion

Use this initializer to load SpriteKit scenes (`.sks` files) created in the Xcode SpriteKit scene editor that contain associated GameplayKit entities, components, and pathfinding graphs.

For more information, see GameplayKit Programming Guide.

