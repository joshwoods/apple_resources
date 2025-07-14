

- SceneKit
- SCNNode
-  opacity 

Instance Property

# opacity

The opacity value of the node. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var opacity: CGFloat { get set }
```

## Mentioned in 

Animating SceneKit Content

## Discussion

Possible values are between `0.0` (fully transparent) and `1.0` (fully opaque). The default is `1.0`.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Modifying the Node Visibility

var isHidden: Bool

A Boolean value that determines the visibility of the node’s contents. Animatable.

var renderingOrder: Int

The order the node’s content is drawn in relative to that of other nodes.

var castsShadow: Bool

A Boolean value that determines whether SceneKit renders the node’s contents into shadow maps.

var movabilityHint: SCNMovabilityHint

A value that indicates how SceneKit should handle the node when rendering movement-related effects.

enum SCNMovabilityHint

Values that inform SceneKit’s rendering for movement-related effects, used by the movabilityHint property.

