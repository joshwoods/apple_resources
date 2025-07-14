

- SceneKit
-  SCNMovabilityHint 

Enumeration

# SCNMovabilityHint

Values that inform SceneKit’s rendering for movement-related effects, used by the movabilityHint property.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum SCNMovabilityHint
```

## Topics

### Constants

case fixed

The node is not expected to move over time.

case movable

The node is expected to move over time.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Modifying the Node Visibility

var isHidden: Bool

A Boolean value that determines the visibility of the node’s contents. Animatable.

var opacity: CGFloat

The opacity value of the node. Animatable.

var renderingOrder: Int

The order the node’s content is drawn in relative to that of other nodes.

var castsShadow: Bool

A Boolean value that determines whether SceneKit renders the node’s contents into shadow maps.

var movabilityHint: SCNMovabilityHint

A value that indicates how SceneKit should handle the node when rendering movement-related effects.

