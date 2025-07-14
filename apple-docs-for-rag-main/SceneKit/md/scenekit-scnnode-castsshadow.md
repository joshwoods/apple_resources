

- SceneKit
- SCNNode
-  castsShadow 

Instance Property

# castsShadow

A Boolean value that determines whether SceneKit renders the node’s contents into shadow maps.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var castsShadow: Bool { get set }
```

## Discussion

SceneKit renders shadows by rendering a *shadow map* image containing silhouettes of the scene’s contents, and then projecting that image onto the scene. SceneKit performs this process once for each SCNLight object in the scene whose castsShadow property is true. Because shadow map rendering re-renders portions of the scene, it incurs a performance cost. To minimize this performance cost, exclude nodes from shadow map rendering by setting the node’s castsShadow property to false.

For more details on shadow rendering, see SCNLight.

## See Also

### Modifying the Node Visibility

var isHidden: Bool

A Boolean value that determines the visibility of the node’s contents. Animatable.

var opacity: CGFloat

The opacity value of the node. Animatable.

var renderingOrder: Int

The order the node’s content is drawn in relative to that of other nodes.

var movabilityHint: SCNMovabilityHint

A value that indicates how SceneKit should handle the node when rendering movement-related effects.

enum SCNMovabilityHint

Values that inform SceneKit’s rendering for movement-related effects, used by the movabilityHint property.

