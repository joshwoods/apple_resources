

- SceneKit
- SCNShaderModifierEntryPoint
-  fragment 

Type Property

# fragment

Use this entry point to change the color of a fragment after all other shading has been performed.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
static let fragment: SCNShaderModifierEntryPoint
```

## Discussion

Shader modifiers for this entry point execute in the fragment processing stage.

The fragment entry point defines the following structure:

```
struct SCNShaderOutput {
   vec4 color;
} _output;
```

Your shader modifier reads from this structure and writes a new color to the same structure to produce the final output color for each rendered fragment.

This shader modifier inverts the output color:

```
_output.color.rgb = vec3(1.0) - _output.color.rgb;
```

## See Also

### Type Properties

static let geometry: SCNShaderModifierEntryPoint

Use this entry point to deform a geometry’s surface or alter its vertex attributes.

static let lightingModel: SCNShaderModifierEntryPoint

Use this entry point to provide a custom lighting equation.

static let surface: SCNShaderModifierEntryPoint

Use this entry point to modify the surface properties of a material before lighting is computed.

