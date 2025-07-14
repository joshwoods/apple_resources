

- SpriteKit
- SKView
-  presentScene(\_:) 

Instance Method

# presentScene(\_:)

Presents a scene.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
func presentScene(_ scene: SKScene?)
```

## Parameters 

`scene`  

The scene to present.

## Mentioned in 

Drawing SpriteKit Content in a View

Responding to Frame-Cycle Events

## Discussion

The new scene immediately replaces the current scene, if one exists.

## See Also

### Displaying a Scene

var scene: SKScene?

The scene currently presented by this view.

func presentScene(SKScene, transition: SKTransition)

Transitions from the current scene to a new scene.

class SKTransition

An object used to perform an animated transition to a new scene.

