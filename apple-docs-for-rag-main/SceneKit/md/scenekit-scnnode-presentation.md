

- SceneKit
- SCNNode
-  presentation 

Instance Property

# presentation

A node object representing the state of the node as it currently appears onscreen.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var presentation: SCNNode { get }
```

## Discussion

When you use implicit animation (see SCNTransaction) to change a node’s properties, those node properties are set immediately to their target values, even though the animated node content appears to transition from the old property values to the new. During the animation SceneKit maintains a copy of the node, called the **presentation node**, whose properties reflect the transitory values determined by any in-flight animations currently affecting the node. The presentation node’s properties provide a close approximation to the version of the node that is currently displayed. SceneKit also uses the presentation node when computing the results of explicit animations, physics, and constraints.

Do not modify the properties of the presentation node. (Attempting to do so results in undefined behavior.) Instead, you use the presentation node to read current animation values—for example, to create a new animation starting at those values.

The presentation node has no parent or child nodes. To access animated properties of related nodes, use the node’s own parent and childNodes properties and the presentation property of each related node.

## See Also

### Working with Node Animation

var isPaused: Bool

A Boolean value that determines whether to run actions and animations attached to the node and its child nodes.

