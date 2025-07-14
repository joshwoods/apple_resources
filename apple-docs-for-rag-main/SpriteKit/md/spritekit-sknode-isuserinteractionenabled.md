

- SpriteKit
- SKNode
-  isUserInteractionEnabled 

Instance Property

# isUserInteractionEnabled

A Boolean value that indicates whether the node receives touch events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var isUserInteractionEnabled: Bool { get set }
```

**watchOS**

``` source
var isUserInteractionEnabled: Bool { get set }
```

## Mentioned in 

Controlling User Interaction on Nodes

Understanding Hit-Testing

## Discussion

The default value is false.

Important

In addition to setting `isUserInteractionEnabled` to `true`, you must subclass the node and define event callbacks in order to respond to user input.

## See Also

### Handling User Input

Controlling User Interaction on Nodes

Enable your node to respond to user input, like touches or mouse clicks.

var focusBehavior: SKNodeFocusBehavior

The focus behavior for a node.

