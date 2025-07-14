

- SpriteKit
- SKScene
-  didMove(to:) 

Instance Method

# didMove(to:)

Tells you when the scene is presented by a view.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
func didMove(to view: SKView)
```

## Parameters 

`view`  

The view that is presenting the scene.

## Discussion

This method is intended to be overridden in a subclass. You can use this method to implement any custom behavior for your scene when it is about to be presented by a view. For example, you might use this method to create the scene’s contents.

## See Also

### Responding to Loading and Resizing Events

func sceneDidLoad()

Tells you when the scene is presented.

func didChangeSize(CGSize)

Tells you when the scene’s size has changed.

func willMove(from: SKView)

Tells you when the scene is about to be removed from a view.

