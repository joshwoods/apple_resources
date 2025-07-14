

- SpriteKit
- SKShapeNode
-  fillShader 

Instance Property

# fillShader

A custom shader used to determine the color of the filled portion of the shape node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var fillShader: SKShader? { get set }
```

**watchOS**

``` source
var fillShader: SKShader? { get set }
```

## Mentioned in 

Controlling Shape Drawing with Shaders

## Discussion

The default value is `nil`. If a `fillShader` is specified, when the shape node is drawn, the shader is used to determine the output colors for any part of the shape node that’s fillled. SpriteKit implements many fill features using a default shader, such as:

- Fill color.

- Animations on alpha.

- Light cast by SKLightNode.

If you supply a custom value for `fillShader`, your custom shader overrides the default shader which neutralizes the default features. It is the responsibility of your custom fillShader to implement any of the features your shape requires.

## See Also

### Customizing Stroking or Fill Drawing

Controlling Shape Drawing with Shaders

Change a shape node’s appearance by supplying custom shader code.

var strokeShader: SKShader?

A custom shader used to determine the color of the stroked portion of the shape node.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

The value of a shader attribute.

