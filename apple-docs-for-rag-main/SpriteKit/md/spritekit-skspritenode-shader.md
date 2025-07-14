

- SpriteKit
- SKSpriteNode
-  shader 

Instance Property

# shader

A text file that defines code that does custom per-pixel drawing or colorization.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var shader: SKShader? { get set }
```

**watchOS**

``` source
var shader: SKShader? { get set }
```

## Mentioned in 

Applying Shaders to a Sprite

## Discussion

The default value is `nil`, which means the default behavior for sprite rendering is performed. SpriteKit implements many sprite features using a default shader, such as:

- Animations on alpha.

- `SKTexture` filteringMode.

- Light from SKLightNode.

If you supply a custom value for `shader`, your custom shader overrides the default shader which neutralizes the default features. It is the responsibility of your custom shader to implement any of the features your sprites require.

## See Also

### Adding a Custom Shader to a Sprite

Applying Shaders to a Sprite

Write custom GLSL code that modifies the look of your sprite.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Sets the value of a shader attribute.

