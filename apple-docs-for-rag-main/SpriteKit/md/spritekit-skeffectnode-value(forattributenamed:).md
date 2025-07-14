

- SpriteKit
- SKEffectNode
-  value(forAttributeNamed:) 

Instance Method

# value(forAttributeNamed:)

Gets the value of a shader attribute.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
func value(forAttributeNamed key: String) -> SKAttributeValue?
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func value(forAttributeNamed key: String) -> SKAttributeValue?
```

## Parameters 

`key`  

The attribute name.

## Return Value

An attribute value object containing the scalar or vector value or `nil` if no such attribute exists.

## See Also

### Applying a Shader with an Effect Node

var shader: SKShader?

A custom shader that is called when the effect node is blended into the parent’s framebuffer.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

