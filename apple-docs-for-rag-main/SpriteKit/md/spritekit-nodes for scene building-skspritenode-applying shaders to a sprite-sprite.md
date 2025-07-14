

- SpriteKit
- Nodes for Scene Building
- SKSpriteNode
-  Applying Shaders to a Sprite 

Article

# Applying Shaders to a Sprite

Write custom GLSL code that modifies the look of your sprite.

## Overview

You can use the shader property of a sprite node to change the appearance of a texture with a custom OpenGL ES fragment shader embedded within a SKShader object. Custom shaders offer almost limitless possibilities, from adding blurs and color treatments to textures to generating imagery such as random noise.

The following code shows a small custom shader which inverts the color of a texture while leaving the alpha or transparency unaffected:

- Swift
- Obj-C

```
let negativeShader = SKShader(source: "void main() { " +
    "    gl_FragColor = vec4(1.0 - SKDefaultShading().rgb, SKDefaultShading().a); " +
    "}")
rocket.shader = negativeShader
```

```
void main() {

    gl_FragColor = vec4(1.0 - SKDefaultShading().rgb, SKDefaultShading().a);
}
```

The following figure illustrates the effect of the shader. The original image, on the left, has its colors inverted by the shader:

## See Also

### Adding a Custom Shader to a Sprite

var shader: SKShader?

A text file that defines code that does custom per-pixel drawing or colorization.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Sets the value of a shader attribute.

