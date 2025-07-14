

- SpriteKit
- SKNode
-  value(forAttributeNamed:) Deprecated

Instance Method

# value(forAttributeNamed:)

The value of a shader attribute.

iOS 10.0–10.0DeprecatediPadOS 10.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.12DeprecatedtvOS 10.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func value(forAttributeNamed key: String) -> SKAttributeValue?
```

**watchOS**

``` source
func value(forAttributeNamed key: String) -> SKAttributeValue?
```

Deprecated

Attributes are only available to node classes supporting SKShader, such as SKSpriteNode, SKEffectNode and SKShapeNode.

## Parameters 

`key`  

The attribute name.

## Return Value

An attribute value object containing the scalar or vector value or `nil` if no such attribute exists.

## See Also

### Setting a Node’s Unique Attributes for a Shader

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

Deprecated

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader

Deprecated

