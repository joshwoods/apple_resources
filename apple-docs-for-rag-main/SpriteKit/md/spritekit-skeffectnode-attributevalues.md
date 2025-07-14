

- SpriteKit
- SKEffectNode
-  attributeValues 

Instance Property

# attributeValues

The values of each attribute associated with the node’s attached shader.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var attributeValues: [String : SKAttributeValue] { get set }
```

**watchOS**

``` source
var attributeValues: [String : SKAttributeValue] { get set }
```

## Discussion

All nodes have their own copy of an attribute value and therefore the attribute values can be different per-node across the same SKShader. If instead you need all nodes to share the same value, use SKUniform. Uniforms can change values every frame, but uniforms cannot vary per-node like attributes can.

## See Also

### Applying a Shader with an Effect Node

var shader: SKShader?

A custom shader that is called when the effect node is blended into the parent’s framebuffer.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Gets the value of a shader attribute.

