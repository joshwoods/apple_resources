

- SpriteKit
- SKEffectNode
-  shader 

Instance Property

# shader

A custom shader that is called when the effect node is blended into the parent’s framebuffer.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var shader: SKShader? { get set }
```

**watchOS**

``` source
var shader: SKShader? { get set }
```

## Discussion

The default value is `nil`, meaning that default blending behavior executes. If a shader is specified, it is called when the rasterized image is blended into the parent’s framebuffer.

## See Also

### Applying a Shader with an Effect Node

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Gets the value of a shader attribute.

