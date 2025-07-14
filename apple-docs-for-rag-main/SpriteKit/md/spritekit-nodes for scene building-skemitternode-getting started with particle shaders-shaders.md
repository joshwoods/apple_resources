

- SpriteKit
- Nodes for Scene Building
- SKEmitterNode
-  Getting Started with Particle Shaders 

Article

# Getting Started with Particle Shaders

Provide custom shader code to alter a particle’s look.

## Overview

Use the shader property of an emitter node to change the appearance of a texture with a custom OpenGL ES fragment shader embedded within an SKShader. Custom shaders offer almost limitless possibilities, from adding blurs and color treatments to textures, to generating imagery such as random noise.

The following code shows a custom shader that renders particles with a radial gradient. The center of each particle is opaque white and the edges are transparent black.

```
let emitter = SKEmitterNode()

let radialGradientShader = SKShader(source: "void main() {" +
    "    vec2 coord = (v_tex_coord - 0.5) * 2.0;" +
    "    gl_FragColor = vec4(1.0 - length(coord));" +
    "}")  

emitter.shader = radialGradientShader
```

## See Also

### Taking Full Control of Particle Drawing with a Shader

var shader: SKShader?

A custom shader used to determine how particles are rendered.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Gets the value of a shader attribute.

