

- SpriteKit
- SKShapeNode
-  strokeShader 

Instance Property

# strokeShader

A custom shader used to determine the color of the stroked portion of the shape node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
var strokeShader: SKShader? { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var strokeShader: SKShader? { get set }
```

## Mentioned in 

Controlling Shape Drawing with Shaders

## Discussion

The default value is `nil`. If a `strokeShader` is specified, when the shape node is drawn, the shader is used to determine the output colors for any part of the shape node that’s stroked. SpriteKit implements many stroke features using a default shader, such as:

- lineCap

- glowWidth

- strokeColor

If you supply a custom value for `strokeShader`, your custom shader overrides the default shader which neutralizes the default features. It is the responsibility of your custom `strokeShader` to implement any of the features your shape requires.

## See Also

### Customizing Stroking or Fill Drawing

Controlling Shape Drawing with Shaders

Change a shape node’s appearance by supplying custom shader code.

var fillShader: SKShader?

A custom shader used to determine the color of the filled portion of the shape node.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

The value of a shader attribute.

