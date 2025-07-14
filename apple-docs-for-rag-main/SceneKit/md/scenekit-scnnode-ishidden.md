

- SceneKit
- SCNNode
-  isHidden 

Instance Property

# isHidden

A Boolean value that determines the visibility of the node’s contents. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var isHidden: Bool { get set }
```

## Discussion

The default value of this property is NO, specifying that SceneKit should render geometries and use lights attached to the node or its children. Change this property’s value to true to exclude attached geometries and lights from rendering. (Cameras attached to the node or its children are not affected by this property.) Hiding a node also hides its child nodes recursively.

You can animate changes to this property’s value. See Animating SceneKit Content. Hiding or showing a node in an animation results in a fade-in or fade-out effect.

## See Also

### Modifying the Node Visibility

var opacity: CGFloat

The opacity value of the node. Animatable.

var renderingOrder: Int

The order the node’s content is drawn in relative to that of other nodes.

var castsShadow: Bool

A Boolean value that determines whether SceneKit renders the node’s contents into shadow maps.

var movabilityHint: SCNMovabilityHint

A value that indicates how SceneKit should handle the node when rendering movement-related effects.

enum SCNMovabilityHint

Values that inform SceneKit’s rendering for movement-related effects, used by the movabilityHint property.

