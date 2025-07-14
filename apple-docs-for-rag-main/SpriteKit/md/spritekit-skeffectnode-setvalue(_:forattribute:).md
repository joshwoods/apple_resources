

- SpriteKit
- SKEffectNode
-  setValue(\_:forAttribute:) 

Instance Method

# setValue(\_:forAttribute:)

Sets an attribute value for an attached shader.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
func setValue(
    _ value: SKAttributeValue,
    forAttribute key: String
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func setValue(
    _ value: SKAttributeValue,
    forAttribute key: String
)
```

## Parameters 

`value`  

An attribute value object containing the scalar or vector value to set in the attached shader.

`key`  

The attribute name.

## See Also

### Applying a Shader with an Effect Node

var shader: SKShader?

A custom shader that is called when the effect node is blended into the parent’s framebuffer.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Gets the value of a shader attribute.

