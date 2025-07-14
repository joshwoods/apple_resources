

- SpriteKit
- SKScene
-  Creating a Scene from a File 

Article

# Creating a Scene from a File

Load a scene that you configure in Xcode’s scene editor.

## Overview

The most common way to load an SKScene is through an `.sks` file configured in Xcode’s scene editor. Making your base changes in the editor is faster than writing equivalent initalization code, and it avoids repeating code if you create a scene in multiple places.

### Create a New Scene File

First, add a new scene file to your project through Xcode’s File menu \> New… \> File \> (choose your platform tab) \> SpriteKit Scene.

### Configure the Scene Using the Editor

You configure your scene in the scene editor by clicking on the `.sks` file in Xcode’s file navigator pane, then adjusting properties in the Utility pane. For example, to set your scene’s background color, follow the steps highlighted in the figure below:

1.  Select the `.sks` file in the file navigator pane.

2.  Open the Utilities pane.

3.  Choose the Attributes inspector.

4.  Define a color under Scene.

### Load the Scene in Code

Load the newly configured scene file in code using init(fileNamed:).

```
let scene = SKScene(fileNamed: "MyScene")

// Now present the scene in a view.
skView.presentScene(scene)
```

Note

The `.sks` file extension is left out of the `String` name argument to init(fileNamed:).

