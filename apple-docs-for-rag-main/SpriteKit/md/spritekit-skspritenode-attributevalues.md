

- SpriteKit
- SKSpriteNode
-  attributeValues 

Instance Property

# attributeValues

The values of each attribute associated with the node’s attached shader.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
var attributeValues: [String : SKAttributeValue] { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var attributeValues: [String : SKAttributeValue] { get set }
```

## Discussion

All nodes have their own copy of an attribute value and therefore the attribute values can be different per-node across the same SKShader. If instead you need all nodes to share the same value, use SKUniform. Uniforms can change values every frame, but uniforms cannot vary per-node like attributes can.

## See Also

### Adding a Custom Shader to a Sprite

Applying Shaders to a Sprite

Write custom GLSL code that modifies the look of your sprite.

var shader: SKShader?

A text file that defines code that does custom per-pixel drawing or colorization.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Sets the value of a shader attribute.

