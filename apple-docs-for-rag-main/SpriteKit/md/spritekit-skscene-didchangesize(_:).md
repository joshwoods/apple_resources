

- SpriteKit
- SKScene
-  didChangeSize(\_:) 

Instance Method

# didChangeSize(\_:)

Tells you when the scene’s size has changed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func didChangeSize(_ oldSize: CGSize)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func didChangeSize(_ oldSize: CGSize)
```

## Parameters 

`oldSize`  

The old size of the scene, in points.

## Mentioned in 

Scaling a Scene’s Content to Fit the View

## Discussion

This method is intended to be overridden in a subclass. Typically, you use this method to adjust the positions of nodes in the scene.

## See Also

### Responding to Loading and Resizing Events

func sceneDidLoad()

Tells you when the scene is presented.

func willMove(from: SKView)

Tells you when the scene is about to be removed from a view.

func didMove(to: SKView)

Tells you when the scene is presented by a view.

