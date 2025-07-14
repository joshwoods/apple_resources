

- SpriteKit
- SKScene
-  willMove(from:) 

Instance Method

# willMove(from:)

Tells you when the scene is about to be removed from a view.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
func willMove(from view: SKView)
```

## Parameters 

`view`  

The view that is presenting the scene.

## Discussion

This method is intended to be overridden in a subclass. You can use this method to implement any custom behavior for your scene when it is about to be removed from the view.

## See Also

### Responding to Loading and Resizing Events

func sceneDidLoad()

Tells you when the scene is presented.

func didChangeSize(CGSize)

Tells you when the scene’s size has changed.

func didMove(to: SKView)

Tells you when the scene is presented by a view.

