

- SpriteKit
- SKNode
-  attributeValues Deprecated

Instance Property

# attributeValues

The values of each attribute associated with the node’s attached shader.

iOS 10.0–10.0DeprecatediPadOS 10.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.12DeprecatedtvOS 10.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

**watchOS**

``` source
var attributeValues: [String : SKAttributeValue] { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var attributeValues: [String : SKAttributeValue] { get set }
```

Deprecated

Attributes are only available to node classes supporting SKShader, such as SKSpriteNode, SKEffectNode and SKShapeNode.

## Discussion

All nodes have their own copy of an attribute value and therefore the attribute values can be different across the same `SKShader`. If instead you need all nodes to share the same value, use `SKUniform`. Uniforms can change values every frame, but uniforms cannot vary per-node like attributes can.

## See Also

### Setting a Node’s Unique Attributes for a Shader

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader

Deprecated

func value(forAttributeNamed: String) -> SKAttributeValue?

The value of a shader attribute.

Deprecated

