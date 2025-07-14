

- SpriteKit
- SKEmitterNode
-  shader 

Instance Property

# shader

A custom shader used to determine how particles are rendered.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var shader: SKShader? { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var shader: SKShader? { get set }
```

## Discussion

The default value is `nil`. If a shader is specified, then the shader is used to determine the output colors for any of the emitter’s particles.

## See Also

### Taking Full Control of Particle Drawing with a Shader

Getting Started with Particle Shaders

Provide custom shader code to alter a particle’s look.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Gets the value of a shader attribute.

