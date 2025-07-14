

- WatchKit
- WKInterfaceSKScene
-  presentScene(\_:) 

Instance Method

# presentScene(\_:)

Presents a scene.

watchOS 3.0+

``` source
func presentScene(_ scene: SKScene?)
```

## Parameters 

`scene`  

The scene to present.

## Discussion

The new scene immediately replaces the current scene, if one exists.

## See Also

### Displaying a Scene

var scene: SKScene?

The currently presented SpriteKit scene.

func presentScene(SKScene, transition: SKTransition)

Transitions from the current scene to a new scene.

