

- SpriteKit
- SKShapeNode
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

All nodes have their own copy of an attribute value and therefore the attribute values can be different across the same SKShader. If instead you need all nodes to share the same value, use SKUniform. Uniforms can change values every frame, but uniforms cannot vary per-node like attributes can.

## See Also

### Customizing Stroking or Fill Drawing

Controlling Shape Drawing with Shaders

Change a shape node’s appearance by supplying custom shader code.

var strokeShader: SKShader?

A custom shader used to determine the color of the stroked portion of the shape node.

var fillShader: SKShader?

A custom shader used to determine the color of the filled portion of the shape node.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

The value of a shader attribute.

