

- SpriteKit
-  SKSceneDelegate 

Protocol

# SKSceneDelegate

Methods that, when implemented, allow any class to participate in the SpriteKit render loop callbacks.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
protocol SKSceneDelegate : NSObjectProtocol
```

## Mentioned in 

Use SpriteKit Objects within Scene Delegate Callbacks

Subclassing Scenes Versus Assigning a Delegate

Displaying 3D Content in a SpriteKit Scene

Getting Started with Nodes

Configuring a Physics Body

## Overview

The SKSceneDelegate protocol is used to implement a delegate to be called whenever the scene is being animated. Typically, you supply a delegate when you want to use a scene without requiring the scene to be subclassed. The methods in this protocol all correspond to methods implemented by the SKScene class. If the delegate implements a particular method, that method is called instead of the corresponding method on the scene object.

When processing a scene, SpriteKit runs a loop that processes and renders the scene. The SKSceneDelegate methods allows you to add logic at any step of the loop.

Important

If your view has a SKViewDelegate and its view(_:shouldRenderAtTime:) method returns false, the update is skipped and none of the scene delegate methods are called.

## Topics

### Handling Animation Events

Use SpriteKit Objects within Scene Delegate Callbacks

Follow threading guidelines to keep your SpriteKit app thread safe.

func update(TimeInterval, for: SKScene)

Tells you to perform any app specific logic to update your scene.

func didEvaluateActions(for: SKScene)

Tells you to peform any necessary logic after scene actions are evaluated.

func didSimulatePhysics(for: SKScene)

Tells you to peform any necessary logic after physics simulations are performed.

func didApplyConstraints(for: SKScene)

Tells you to peform any necessary logic after constraints are applied.

func didFinishUpdate(for: SKScene)

Tells you to peform any necessary logic after the scene has finished all of the steps required to process animations.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Configuring a Delegate

Subclassing Scenes Versus Assigning a Delegate

Use a scene delegate to share app logic across various scenes.

var delegate: (any SKSceneDelegate)?

A delegate to be called during the animation loop.

