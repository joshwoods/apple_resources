

- SpriteKit
-  SKEmitterNode 

Class

# SKEmitterNode

A source of various particle effects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
class SKEmitterNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKEmitterNode
```

## Mentioned in 

Using Keyframe Sequence to effect Custom Interpolation

Creating Particle Effects

Animating Particle Properties Across Disparate Values

Animate the Warping of a Sprite

## Overview

A SKEmitterNode object is a node that automatically creates and renders small particle sprites. Particles are privately owned by SpriteKit—your game cannot access the generated sprites. For example, you cannot add physics shapes to particles. Emitter nodes are often used to create smoke, fire, sparks, and other particle effects. A *particle* is similar to an SKSpriteNode object; it renders a textured or untextured image that is sized, colorized, and blended into the scene. However, particles differ from sprites in two important ways:

- A particle’s texture is always stretched uniformly.

- Particles are not represented by objects in SpriteKit. This means you cannot perform node-related tasks on particles, nor can you associate physics bodies with particles to make them interact with other content. Although there is no visible class representing particles added by the emitter node, you can think of a particle as having properties like any other object.

Particles are purely visual objects, and their behavior is entirely defined by the emitter node that created them. The emitter node contains many properties to control the behavior of the particles it generates, including:

- The birth rate and lifetime of the particle. You can also specify the order in which the particles are rendered and the maximum number of particles that are created before the emitter turns itself off.

- The starting values of the particle, including its position, orientation, color, and size. You can choose to have these starting values randomized.

- The changes to apply to the particle over its lifetime. Typically, these are specified as a rate of change over time. For example, you might specify that a particle rotates at a particular rate, in radians per second. The emitter automatically updates the particle data for each frame. In most cases, you can also create more sophisticated behaviors using keyframe sequences. For example, you might specify a keyframe sequence for a particle so that it starts out small, scales up to a larger size, then shrinks before dying.

## Topics

### First Steps

Creating Particle Effects

Add particle effects to your app by creating repeatable particles in Xcode’s editor, or in code.

### Choosing Which Node in the Scene Emits Particles

Choose which node in the scene emits particles.

Changing the Location of Particles in Your Scene

Set a target node from which SpriteKit creates particles.

var targetNode: SKNode?

The target node that renders the emitter’s particles.

### Controlling When Particles Are Created

func advanceSimulationTime(TimeInterval)

Advances the emitter particle simulation.

func resetSimulation()

Removes all existing particles and restarts the simulation.

var particleBirthRate: CGFloat

The rate at which new particles are created.

var numParticlesToEmit: Int

The number of particles the emitter should emit before stopping.

### Controlling the Rendering Order of an Emitter’s Particles

var particleRenderOrder: SKParticleRenderOrder

The order in which the emitter’s particles are rendered.

enum SKParticleRenderOrder

The order to use when the emitter’s particles are rendered.

### Controlling Particle Lifetime

var particleLifetime: CGFloat

The average lifetime of a particle, in seconds.

var particleLifetimeRange: CGFloat

The range of allowed random values for a particle’s lifetime.

### Controlling Particle Position

var particlePosition: CGPoint

The average starting position for a particle.

var particlePositionRange: CGVector

The range of allowed random values for a particle’s position.

var particleZPosition: CGFloat

The average starting depth of a particle.

var particleZPositionRange: CGFloat

The range of allowed random values for a particle’s depth.

### Controlling Particle Velocity and Acceleration

var particleSpeed: CGFloat

The average initial speed of a new particle, in points per second.

var particleSpeedRange: CGFloat

The range of allowed random values for a particle’s initial speed.

var emissionAngle: CGFloat

The average initial direction of a particle, expressed as an angle in radians.

var emissionAngleRange: CGFloat

The range of allowed random values for a particle’s initial direction, expressed as an angle in radians.

var xAcceleration: CGFloat

The acceleration to apply to a particle’s horizontal velocity.

var yAcceleration: CGFloat

The acceleration to apply to a particle’s vertical velocity.

var particleZPositionSpeed: CGFloat

The speed at which the particle’s depth changes.

### Adjusting a Particle’s Rotation

var particleRotation: CGFloat

The average initial rotation of a particle, expressed as an angle in radians.

var particleRotationRange: CGFloat

The range of allowed random values for a particle’s initial rotation, expressed as an angle in radians.

var particleRotationSpeed: CGFloat

The speed at which a particle rotates, expressed in radians per second.

### Scaling Particles by a Factor

var particleScale: CGFloat

The average initial scale factor of a particle.

var particleScaleRange: CGFloat

The range of allowed random values for a particle’s initial scale.

var particleScaleSpeed: CGFloat

The rate at which a particle’s scale factor changes per second.

var particleScaleSequence: SKKeyframeSequence?

The sequence used to specify the scale factor of a particle over its lifetime.

### Changing a Particle’s Source Image and Size

var particleTexture: SKTexture?

The texture to use to render a particle.

var particleSize: CGSize

The starting size of each particle.

### Configuring Particle Color

var particleColorSequence: SKKeyframeSequence?

The sequence used to specify the color components of a particle over its lifetime.

var particleColor: UIColor

The average initial color for a particle.

var particleColorAlphaRange: CGFloat

The range of allowed random values for the alpha component of a particle’s initial color.

var particleColorBlueRange: CGFloat

The range of allowed random values for the blue component of a particle’s initial color.

var particleColorGreenRange: CGFloat

The range of allowed random values for the green component of a particle’s initial color.

var particleColorRedRange: CGFloat

The range of allowed random values for the red component of a particle’s initial color.

var particleColorAlphaSpeed: CGFloat

The rate at which the alpha component of a particle’s color changes per second.

var particleColorBlueSpeed: CGFloat

The rate at which the blue component of a particle’s color changes per second.

var particleColorGreenSpeed: CGFloat

The rate at which the green component of a particle’s color changes per second.

var particleColorRedSpeed: CGFloat

The rate at which the red component of a particle’s color changes per second.

### Controlling How the Texture is Blended with Particle Color

var particleColorBlendFactorSequence: SKKeyframeSequence?

The sequence used to specify the color blend factor of a particle over its lifetime.

var particleColorBlendFactor: CGFloat

The average starting value for the color blend factor.

var particleColorBlendFactorRange: CGFloat

The range of allowed random values for a particle’s starting color blend factor.

var particleColorBlendFactorSpeed: CGFloat

The rate at which the color blend factor changes per second.

### Blending Particles with the Framebuffer

Change how an emitter uses an alpha value, such as additive blending, that results in the emitter being brighter than it was before.

var particleBlendMode: SKBlendMode

The blending mode used to blend particles into the framebuffer.

var particleAlphaSequence: SKKeyframeSequence?

The sequence used to specify the alpha value of a particle over its lifetime.

var particleAlpha: CGFloat

The average starting alpha value for a particle.

var particleAlphaRange: CGFloat

The range of allowed random values for a particle’s starting alpha value.

var particleAlphaSpeed: CGFloat

The rate at which the alpha value of a particle changes per second.

### Animating Particles

Change particles over time using actions or keyframe sequences.

Animating Particle Properties Across Disparate Values

Supply keyframe sequences to do linear or nonlinear particle animations.

var particleAction: SKAction?

An action executed by new particles.

### Applying Physics Fields to the Particles

var fieldBitMask: UInt32

A mask that defines which categories of physics fields can exert forces on the particles.

### Taking Full Control of Particle Drawing with a Shader

Getting Started with Particle Shaders

Provide custom shader code to alter a particle’s look.

var shader: SKShader?

A custom shader used to determine how particles are rendered.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

func value(forAttributeNamed: String) -> SKAttributeValue?

Gets the value of a shader attribute.

### Maximizing Particle Run-Time Performance

Optimizing Emitter Node Performance

Use proven methods to rapidly create and play back performant particle effects.

## Relationships

### Inherits From

- SKNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable
- UIActivityItemsConfigurationProviding
- UICoordinateSpace
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Nodes that Draw

Maximizing Node Drawing Performance

Structure your nodes for maximum performance.

class SKSpriteNode

An image or solid color.

class SKShapeNode

A mathematical shape that can be stroked or filled.

class SKLabelNode

A graphical element that draws text.

class SKVideoNode

A graphical element that plays video content.

class SKTileMapNode

A two-dimensional array of images.

class SK3DNode

3D SceneKit content drawn as a flattened sprite.

