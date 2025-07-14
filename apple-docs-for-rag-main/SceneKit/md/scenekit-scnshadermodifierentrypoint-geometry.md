

- SceneKit
- SCNShaderModifierEntryPoint
-  geometry 

Type Property

# geometry

Use this entry point to deform a geometry’s surface or alter its vertex attributes.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
static let geometry: SCNShaderModifierEntryPoint
```

## Discussion

Shader modifiers for this entry point execute in the vertex processing stage.

The geometry entry point declares the following structure:

```
struct SCNShaderGeometry {
   vec3 position;
   vec3 normal;
   vec4 tangent;
   vec2 texcoords[kSCNTexcoordCount];
} _geometry;
```

Your shader modifier reads from this structure and writes new values to the same structure to alter the geometric properties of each vertex in a geometry.

The `position`, `normal`, and `tangent` fields are expressed in model space. You can use SceneKit’s uniforms (such as `u_modelViewTransform`) to operate in a different coordinate space, but you must convert back to model space before writing results.

The `kSCNTexcoordCount` variable is a constant integer corresponding to the geometry’s number of texture coordinate sources. Each set of coordinates in the `texcoords` field contains raw values from the geometry—SceneKit applies the contentsTransform transformation (if any) after the geometry shader modifier completes.

The below shader modifier produces an animated sinusoidal deformation:

```
uniform float Amplitude = 0.1;

_geometry.position +=
    _geometry.normal *
    (Amplitude*_geometry.position.y*_geometry.position.x) *
    sin(1.0 * u_time);
```

## See Also

### Type Properties

static let fragment: SCNShaderModifierEntryPoint

Use this entry point to change the color of a fragment after all other shading has been performed.

static let lightingModel: SCNShaderModifierEntryPoint

Use this entry point to provide a custom lighting equation.

static let surface: SCNShaderModifierEntryPoint

Use this entry point to modify the surface properties of a material before lighting is computed.

