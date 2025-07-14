

- SpriteKit
- SKScene
-  sceneDidLoad() 

Instance Method

# sceneDidLoad()

Tells you when the scene is presented.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func sceneDidLoad()
```

**watchOS**

``` source
func sceneDidLoad()
```

## Mentioned in 

Controlling User Interaction on Nodes

## Discussion

This method is intended to be overridden in a subclass. It is the preferred location to peform custom setup after the scene has been initialized or decoded.

## See Also

### Responding to Loading and Resizing Events

func didChangeSize(CGSize)

Tells you when the scene’s size has changed.

func willMove(from: SKView)

Tells you when the scene is about to be removed from a view.

func didMove(to: SKView)

Tells you when the scene is presented by a view.

