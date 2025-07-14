

- SpriteKit
-  Drawing SpriteKit Content in a View 

Article

# Drawing SpriteKit Content in a View

Display visual content using SpriteKit.

## Overview

Display SpriteKit content on the screen by configuring a SpriteKit renderer, its scene, and the visual objects you lay out on top of the scene. SpriteKit provides objects that are designed specifically for various types of content (see Nodes for Scene Building), but for simplicity, this article displays an image in a view.

Note

There are other ways to draw SpriteKit content besides using a view. See Choosing a SpriteKit Scene Renderer for options.

Because the code in this article sets up a view, you put the lines from each of the following code listings into a view controller’s viewDidLoad() function.

### Create the Scene

Everything displayed with SpriteKit is done through a scene object, which is an instance of SKScene. Use the following code to set up a basic scene:

```
```

When you pass the `size` of the view’s `bounds` to the scene initializer, you size the scene to the view’s size. When you set the scene’s anchorPoint to `(0.5, 0.5)`, you determine that the coordinates (0, 0) map to the center of the view.

For further discussion about how setting the `anchorPoint` changes an object’s position in the view, see Using the Anchor Point to Move the Sprite’s Frame.

### Lay Out Visual Content on Top of the Scene

You use node objects to display graphics in a SpriteKit view. SpriteKit provides different nodes depending on the content (see Nodes that Draw in Nodes for Scene Building). In this case, use an SKSpriteNode to display an image in the view:

```
```

The functions to lay out content in a scene are covered in more detail in Accessing and Modifying the Node Tree.

### Present the Scene Inside a View

After you set up the scene, you display it in the view by calling presentScene(_:):

```
```

Because the code in this article sets up a view, you add it to your view controller’s viewDidLoad() function.

## See Also

### Essentials

class SKScene

An object that organizes all of the active SpriteKit content.

Nodes for Scene Building

Define the appearance or layout of scene content.

