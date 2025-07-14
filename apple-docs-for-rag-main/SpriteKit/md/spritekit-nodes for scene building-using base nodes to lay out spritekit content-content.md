

- SpriteKit
- Nodes for Scene Building
-  Using Base Nodes to Lay Out SpriteKit Content 

Article

# Using Base Nodes to Lay Out SpriteKit Content

Use nonvisual nodes to define the layout of a scene.

## Overview

Each onscreen element in SpriteKit is referred to as a *node*. Nodes are either visual elements or containers of other nodes. You set up the appearance of a SpriteKit scene by adding nodes alongside and on top of each other in a hierarchical form. Collectively, this structure is referred to as the *node tree* or the *node hierarchy*.

These are the basic nonvisual nodes in SpriteKit:

- SKNode is a container node. It doesn’t render any content of its own, but works as a layout tool for its child nodes.

- SKReferenceNode doesn’t define content of its own, but refers to another node or archived file that does.

- SKCameraNode defines point of view within a scene. Its inverse scale is applied to all nodes in the hierarchy except for its children. Use the children of `SKCameraNode` for UI elements that should be unaffected by zoom level.

For a list of visual elements, see Nodes that Draw in Nodes for Scene Building, which also includes some examples of using visual nodes.

## See Also

### Base Nodes

class SKNode

The base class of all SpriteKit nodes.

class SKCameraNode

A node that determines which parts of the scene are visible within a view.

class SKReferenceNode

A node that’s defined in an archived `.sks` file.

