

- WatchKit
- WKInterfaceSKScene
-  presentScene(\_:transition:) 

Instance Method

# presentScene(\_:transition:)

Transitions from the current scene to a new scene.

watchOS 3.0+

``` source
func presentScene(
    _ scene: SKScene,
    transition: SKTransition
)
```

## Parameters 

`scene`  

The scene to present.

`transition`  

A transition used to animate between the two scenes.

## Discussion

If the interface is not currently presenting a scene, the new scene is presented immediately, and the `transition` property is ignored. Otherwise, the interface’s scene property is updated immediately, and the transition is executed to animate the swap between scenes.

## See Also

### Displaying a Scene

var scene: SKScene?

The currently presented SpriteKit scene.

func presentScene(SKScene?)

Presents a scene.

