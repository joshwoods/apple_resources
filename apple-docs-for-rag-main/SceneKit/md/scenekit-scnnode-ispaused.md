

- SceneKit
- SCNNode
-  isPaused 

Instance Property

# isPaused

A Boolean value that determines whether to run actions and animations attached to the node and its child nodes.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isPaused: Bool { get set }
```

## Discussion

The default value of this property is false, specifying that SceneKit should continuously update the node’s contents. Pausing a node pauses any running animations or actions. This property applies to the actions and animations attached to the node itself and those attached to any of its child or descendant nodes.

## See Also

### Working with Node Animation

var presentation: SCNNode

A node object representing the state of the node as it currently appears onscreen.

