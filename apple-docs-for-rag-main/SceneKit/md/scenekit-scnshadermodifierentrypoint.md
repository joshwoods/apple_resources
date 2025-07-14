

- SceneKit
-  SCNShaderModifierEntryPoint 

Structure

# SCNShaderModifierEntryPoint

Keys for the shaderModifiers dictionary, each corresponding to an entry point in SceneKit’s shader programs where you can attach a custom GPU shader code snippet.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SCNShaderModifierEntryPoint
```

## Discussion

For details on shader modifiers, see Use Shader Modifiers to Extend SceneKit Shading in the protocol overview.

SceneKit inserts your shader modifiers into its shader program in the order shown here, so you can use the structures defined by earlier entry points in later entry points. For example, a snippet associated with the fragment entry point can read from the `_surface` structure defined by the surface entry point.

## Topics

### Type Properties

static let fragment: SCNShaderModifierEntryPoint

Use this entry point to change the color of a fragment after all other shading has been performed.

static let geometry: SCNShaderModifierEntryPoint

Use this entry point to deform a geometry’s surface or alter its vertex attributes.

static let lightingModel: SCNShaderModifierEntryPoint

Use this entry point to provide a custom lighting equation.

static let surface: SCNShaderModifierEntryPoint

Use this entry point to modify the surface properties of a material before lighting is computed.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

typealias SCNBindingBlock

The signature for a block called for binding or unbinding a GLSL symbol in a custom program.

