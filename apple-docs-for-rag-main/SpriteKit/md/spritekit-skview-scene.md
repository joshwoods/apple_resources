

- SpriteKit
- SKView
-  scene 

Instance Property

# scene

The scene currently presented by this view.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
var scene: SKScene? { get }
```

## Mentioned in 

Choosing a SpriteKit Scene Renderer

## Discussion

The default value is `nil`.

You call presentScene(_:) to assign a value to this property.

## See Also

### Displaying a Scene

func presentScene(SKScene?)

Presents a scene.

func presentScene(SKScene, transition: SKTransition)

Transitions from the current scene to a new scene.

class SKTransition

An object used to perform an animated transition to a new scene.

