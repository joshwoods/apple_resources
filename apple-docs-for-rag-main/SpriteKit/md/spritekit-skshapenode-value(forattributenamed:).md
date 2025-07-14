

- SpriteKit
- SKShapeNode
-  value(forAttributeNamed:) 

Instance Method

# value(forAttributeNamed:)

The value of a shader attribute.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func value(forAttributeNamed key: String) -> SKAttributeValue?
```

**watchOS**

``` source
func value(forAttributeNamed key: String) -> SKAttributeValue?
```

## Parameters 

`key`  

The attribute name.

## Return Value

An attribute value object containing the scalar or vector value or `nil` if no such attribute exists.

## See Also

### Customizing Stroking or Fill Drawing

Controlling Shape Drawing with Shaders

Change a shape node’s appearance by supplying custom shader code.

var strokeShader: SKShader?

A custom shader used to determine the color of the stroked portion of the shape node.

var fillShader: SKShader?

A custom shader used to determine the color of the filled portion of the shape node.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

