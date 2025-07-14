

- SpriteKit
- SKLightNode
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the node is casting light.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
var isEnabled: Bool { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

If the value is true, the light is enabled and affects sprite nodes in the scene. The default is true.

## See Also

### Determining Whether a Light Node Is Active

var categoryBitMask: UInt32

A mask that defines which categories this light belongs to.

