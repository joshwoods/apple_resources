

- SpriteKit
- SKSpriteNode
-  setValue(\_:forAttribute:) 

Instance Method

# setValue(\_:forAttribute:)

Sets an attribute value for an attached shader.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

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

## Parameters 

`value`  

An attribute value object containing the scalar or vector value to set in the attached shader.

`key`  

The attribute name.

## See Also

### Adding a Custom Shader to a Sprite

Applying Shaders to a Sprite

Write custom GLSL code that modifies the look of your sprite.

var shader: SKShader?

A text file that defines code that does custom per-pixel drawing or colorization.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Sets the value of a shader attribute.

