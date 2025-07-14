

- SpriteKit
- SKView
-  presentScene(\_:transition:) 

Instance Method

# presentScene(\_:transition:)

Transitions from the current scene to a new scene.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
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

If there is currently a scene presented by the view, the view’s scene property is updated immediately, the transition is executed to swap between the scenes. Otherwise, the new scene is presented immediately and the transition property is ignored.

## See Also

### Displaying a Scene

var scene: SKScene?

The scene currently presented by this view.

func presentScene(SKScene?)

Presents a scene.

class SKTransition

An object used to perform an animated transition to a new scene.

