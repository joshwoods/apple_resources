

- SpriteKit
- SKNode
-  isHidden 

Instance Property

# isHidden

A Boolean value that determines whether a node and its descendants are rendered.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var isHidden: Bool { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var isHidden: Bool { get set }
```

## Mentioned in 

About Node Property Propagation

Getting Started with Nodes

## Discussion

When hidden, a node and its descendants are not rendered. However, they still exist in the scene and continue to interact in other ways. For example, the node’s actions still run and the node can still be intersected with other nodes. The default value is false.

## See Also

### Altering Node Visibility

var alpha: CGFloat

The transparency value applied to the node’s contents.

