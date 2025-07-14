

- SpriteKit
- SKNode
-  setValue(\_:forAttribute:) Deprecated

Instance Method

# setValue(\_:forAttribute:)

Sets an attribute value for an attached shader

iOS 10.0–10.0DeprecatediPadOS 10.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.12DeprecatedtvOS 10.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func setValue(
    _ value: SKAttributeValue,
    forAttribute key: String
)
```

**watchOS**

``` source
func setValue(
    _ value: SKAttributeValue,
    forAttribute key: String
)
```

Deprecated

Attributes are only available to node classes supporting SKShader, such as SKSpriteNode, SKEffectNode and SKShapeNode.

## Parameters 

`value`  

An attribute value object containing the scalar or vector value to set in the attached shader.

`key`  

The attribute name.

## See Also

### Setting a Node’s Unique Attributes for a Shader

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

Deprecated

func value(forAttributeNamed: String) -> SKAttributeValue?

The value of a shader attribute.

Deprecated

