

- WatchKit
-  WKInterfaceSKScene 

Class

# WKInterfaceSKScene

A visual WatchKit element that displays a SpriteKit scene.

watchOS 3.0+

``` source
class WKInterfaceSKScene
```

## Overview

Present a scene by calling the interface’s presentScene(_:) or presentScene(_:transition:) method and passing in a SKScene object. When a scene is presented, it alternates between running its simulation (which animates the content) and rendering the content for display. You can pause the scene by setting the interface’s isPaused property to true.

Do not subclass or create instances of this class yourself. Instead, drag a SpriteKit Scene object from your Object Library and add it to your storyboard. Then define an outlet in your interface controller class and connect it to the SpriteKit Scene object. For example, to refer to a scene object in your interface, define a property with the following syntax in your interface controller class:

- Swift
- Objective-C

```
@IBOutlet weak var sceneInterface: WKInterfaceSKScene!
```

```
@property (weak, nonatomic) IBOutlet WKInterfaceSKScene* sceneInterface;
```

During the initialization of your interface controller, WatchKit creates a new instance of this class and assigns it to your outlet. At that point, you can use the object in your outlet to make changes to the SpriteKit scene.

The SpriteKit scene in your Watch app must be connected to a WKInterfaceSKScene outlet in your WatchKit extension for the scene to be visible in your watchOS app’s user interface.

## Topics

### Displaying a Scene

Define the content displayed by this watch interface.

var scene: SKScene?

The currently presented SpriteKit scene.

func presentScene(SKScene?)

Presents a scene.

func presentScene(SKScene, transition: SKTransition)

Transitions from the current scene to a new scene.

### Configuring the Scene in a Storyboard

Adjust the Storyboard to set up your watch interface.

Configuring a WatchKit Scene in a Storyboard

Xcode lets you configure information about your SpriteKit Scene in your storyboard file. The following table lists the attributes you can configure in your storyboard and their meaning.

### Controlling the Timing of a Scene’s Rendering

Define the display link callback frequency or pause callbacks entirely.

var preferredFramesPerSecond: Int

The animation frame rate that the interface uses to render its scene.

var isPaused: Bool

A Boolean value that determines whether the view’s scene animations are paused.

### Snapshotting Nodes to a Texture

Create a snapshot of a transformed node or portion of the node tree.

func texture(from: SKNode) -> SKTexture?

Renders the contents of a node tree and returns the rendered image as a SpriteKit texture.

func texture(from: SKNode, crop: CGRect) -> SKTexture?

Renders a portion of a node’s contents and returns the rendered image as a SpriteKit texture.

### Initializing for SwiftUI

init()

Creates a SpriteKit scene for use in SwiftUI.

Deprecated

## Relationships

### Inherits From

- WKInterfaceObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Graphics and games

class WKInterfaceSCNScene

An object that lets you manage SceneKit content for display in your app.

