

- SceneKit
- SCNNode
-  renderingOrder 

Instance Property

# renderingOrder

The order the node’s content is drawn in relative to that of other nodes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var renderingOrder: Int { get set }
```

## Discussion

Nodes with greater rendering orders are rendered last. Defaults to zero.

## See Also

### Modifying the Node Visibility

var isHidden: Bool

A Boolean value that determines the visibility of the node’s contents. Animatable.

var opacity: CGFloat

The opacity value of the node. Animatable.

var castsShadow: Bool

A Boolean value that determines whether SceneKit renders the node’s contents into shadow maps.

var movabilityHint: SCNMovabilityHint

A value that indicates how SceneKit should handle the node when rendering movement-related effects.

enum SCNMovabilityHint

Values that inform SceneKit’s rendering for movement-related effects, used by the movabilityHint property.

