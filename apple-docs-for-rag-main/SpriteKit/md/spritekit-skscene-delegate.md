

- SpriteKit
- SKScene
-  delegate 

Instance Property

# delegate

A delegate to be called during the animation loop.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
weak var delegate: (any SKSceneDelegate)? { get set }
```

**watchOS**

``` source
weak var delegate: (any SKSceneDelegate)? { get set }
```

## Discussion

When a delegate is present, when any of the animation loop methods steps are executed, your delegate is called. Typically, you use a delegate when you do not want to implement a scene subclass or if you want to dynamically change the scene behavior at runtime.

## See Also

### Configuring a Delegate

Subclassing Scenes Versus Assigning a Delegate

Use a scene delegate to share app logic across various scenes.

protocol SKSceneDelegate

Methods that, when implemented, allow any class to participate in the SpriteKit render loop callbacks.

