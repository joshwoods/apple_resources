

- SceneKit
-  SCNShadable 

Protocol

# SCNShadable

Methods for customizing SceneKit’s rendering of geometry and materials using Metal or OpenGL shader programs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol SCNShadable : NSObjectProtocol
```

## Overview

SceneKit provides two ways to integrate custom GPU shader programs into the rendering of your scene: program objects and shader modifiers.

### Use Program Objects to Replace SceneKit Shading

For complete control of the vertex and fragment shaders used to render an object, assign an SCNProgram instance to the object’s program property. A custom program completely replaces all other rendering parameters, including material settings. Your custom program takes inputs from SceneKit and is responsible for all transform, lighting, and shading effects you want it to produce. For details on custom programs, see SCNProgram.

When you specify a custom program, you can provide handler blocks that SceneKit calls at render time to update the values of custom variables in your shaders. See the methods in Handling Parameters in Custom OpenGL Shader Programs.

### Use Shader Modifiers to Extend SceneKit Shading

Shader modifiers are an alternative to entirely replacing SceneKit’s shaders with your own. You can use shader modifiers to, for example:

- Parametrically deform the surface of a geometry

- Simulate realistic surfaces with complex material properties

- Add artistic lighting effects such as cartoon-style shading

- Create special effects by post-processing pixels after SceneKit’s shading is complete

A shader modifier is a snippet of source code in the Metal shader language or OpenGL Shader Language (GLSL) that SceneKit injects into its own shader programs at a defined entry point. Because your shader modifiers are additions to SceneKit’s shader program, using shader modifiers leaves SceneKit’s rendering system intact. That is, you can still use material properties, lighting models, and camera effects to affect the rendered image.

You attach a snippet to a SCNGeometry or SCNMaterial object using its shaderModifiers property, associating it with an entry point corresponding to the stage of SceneKit’s shader program that it modifies: geometry, surface, lighting, or fragment. Each entry point defines a context for the associated snippet, with input variables providing SceneKit’s rendering parameters in that stage and output variables that the snippet writes its results to.

For definitions of each entry point and its inputs and outputs, see `Shader Modifier Entry Point Keys`. SceneKit inserts your shader modifiers into its shader program a specific order:

1.  geometry

2.  surface

3.  lightingModel

4.  fragment

You can use the structures defined by earlier entry points in later entry points. For example, a snippet associated with the fragment entry point can read from the `_surface` structure defined by the surface entry point.

#### Writing a Shader Modifier Snippet

The code you provide for a shader modifier must be organized in a specific structure, as illustrated in the example below:

```
// 1. Custom variable declarations (optional)
// For Metal, a pragma directive and one custom variable on each line:
#pragma arguments
float intensity;
// For OpenGL, a separate uniform declaration for each custom variable
uniform float intensity;

// 2. Custom global functions (optional)
vec2 sincos(float t) { return vec2(sin(t), cos(t)); }

// 3. Pragma directives (optional)
#pragma transparent
#pragma body

// 4. Code snippet
_geometry.position.xy = sincos(u_time);
_geometry.position.z = intensity;
```

1.  **Custom variables declarations.** You can provide your own inputs to a shader modifier by declaring custom variables. Because the syntax differs between Metal and OpenGL shaders, you must include both declarations for your shader modifier to be usable with both rendering technologies. To pass values into custom variables at render time, see Providing Custom Inputs to a Shader Modifier.

2.  **Custom global functions.** If your shader modifier benefits from factoring common code into functions, place their definitions here. If you include custom functions in your snippet, you must place the `#pragma body` directive between your function definitions and the main body of the snippet.

3.  **Pragma directives.** As noted above, the `#pragma body` directive separates custom function definitions from the main body of the snippet. If the snippet contains no function definitions, you may omit this directive.

By default, SceneKit automatically uses material properties to determine whether an object should be rendered with partial transparency and uses this information to optimize rendering performance. Use the `#pragma transparent` or `#pragma opaque` directive to override SceneKit’s setting. 4. **Code Snippet.** Place the main body of your shader modifier code at the end of the code snippet.

One shader modifier snippet affects both Metal and OpenGL (or OpenGL ES) rendering—SceneKit automatically translates GLSL syntax to Metal shader syntax before inserting your code snippet into its own shader program. (For some simple shader modifiers, SceneKit can insert the same code snippet into either shader language without translation.)

#### Providing Custom Inputs to a Shader Modifier

You can also declare custom uniform variables in your shader modifier snippet. You provide values for custom uniform variables using Key-value coding. For each uniform variable you declare in a shader modifier attached to an SCNMaterial or SCNGeometry object, SceneKit observes a key with the same name on that object. When you set a new value, SceneKit automatically binds that value to the corresponding uniform location in the shader program. If you animate a change to the value implicitly (with the SCNTransaction class) or explicitly (with the SCNAnimatable protocol), SceneKit interpolates intermediate values and binds them to the uniform for each frame of the animation. For example, the following code animates the fading of a material from full color to grayscale:

```
// Set up the shader modifier with a custom uniform.
myMaterial.shaderModifiers = @{ SCNShaderModifierEntryPointFragment :
    @"uniform float mixLevel = 0.0;"
    "vec3 gray = vec3(dot(vec3(0.3, 0.59, 0.11), _output.color.rgb));"
    "_output.color = mix(_output.color, vec4(gray, 1.0), mixLevel);" };

// Later, animate a change to the uniform.
[SCNTransaction begin];
{
    [myMaterial setValue:@1.0 forKeyPath:@"mixLevel"];
}
[SCNTransaction commit];
```

Because SceneKit binds values to shader variables using Key-value observing, you can provide values in several ways. If you set a value using the setValue(_:forKey:) or setValue(_:forKeyPath:) method, or set a target value for a keypath animation, the value must be contained in an Objective-C object. For uniforms of scalar types, you can assign an NSNumber object as a value. Assigning a uniform of a vector or matrix type requires an NSValue object containing data of the appropriate type. You can also bind textures to texture samplers using SCNMaterialProperty objects.

Alternatively, you can create an SCNMaterial or SCNGeometry subclass for your custom shadable object and declare properties whose names match those of the uniform variables in your shader. When you assign a value to the property, SceneKit automatically binds it to the corresponding uniform in the shader program. In this case, your properties can use primitive or structure types appropriate to the corresponding Metal or GLSL variables.

The table below lists the Objective-C types for each shading language data type:

| GLSL data types | Metal data types | Objective-C type |
|----|----|----|
| `int` | `int` | NSNumber, NSValue (NSInteger, `int`) |
| `float` | `float` | NSNumber, NSValue (CGFloat, `float`, `double`) |
| `vec2` | `float2` | NSValue (CGPoint) |
| `vec3` | `float3` | NSValue (SCNVector3) |
| `vec4` | `float4` | NSValue (SCNVector4) |
| `mat4`  `mat4x4` | `float4x4` | NSValue (CATransform3D) |
| `sampler2D`  `samplerCube` | `sampler` | SCNMaterialProperty |

#### Using Inputs Provided by SceneKit

SceneKit declares the following uniform variables containing global rendering parameters:

| Identifier | GLSL Type | Description |
|----|----|----|
| `u_time` | `float` | The current system time (in seconds) since SceneKit started rendering with the shader. |
| `u_boundingBox` | `mat32` | The bounding box of the geometry being rendered, in model space.  `u_boundingBox[0].xyz` is the minimum corner of the bounding box and `u_boundingBox[1].xyz` is the maximum corner. |
| `u_modelTransform`  `u_viewTransform`  `u_projectionTransform`  `u_normalTransform`  `u_modelViewTransform`  `u_modelViewProjectionTransform` | `mat4` | The transform matrices used for converting vertex positions and normals between model, world, view, and clip coordinate spaces.  For detailed definitions, see Rendering Transform Keys. |
| `u_inverseModelTransform`  `u_inverseViewTransform`  `u_inverseProjectionTransform`  `u_inverseModelViewTransform`  `u_inverseModelViewProjectionTransform` | `mat4` | The inverse matrices corresponding to each transform. |
| `u_diffuseTexture`  `u_ambientTexture`  `u_specularTexture`  `u_normalTexture`  `u_reflectiveTexture`  `u_emissionTexture`  `u_transparentTexture`  `u_multiplyTexture` | `sampler2D` or `samplerCube` | The texture contents of the corresponding material property. Declared only if the material property’s contents object provides a texture image.  The GLSL type of the uniform variable depends on whether the contents are a 2D image or cube map.  For details on materials, see SCNMaterial. |

Shader modifiers may contain any legal Metal shader or GLSL code, with the exception that SceneKit reserves for its own use all identifier names with the `u_`, `a_`, and `v_` prefixes.

## Topics

### Assigning a Custom Shader Program

var program: SCNProgram?

A program used when rendering the object.

### Customizing SceneKit’s Shader Programs

var shaderModifiers: [SCNShaderModifierEntryPoint : String]?

A dictionary of GLSL source code snippets for customizing the shader programs provided by SceneKit.

### Handling Parameters in Custom OpenGL Shader Programs

func handleBinding(ofSymbol: String, handler: SCNBindingBlock?)

Specifies a block to be called before rendering with programs with the specified GLSL uniform variable or attribute name.

func handleUnbinding(ofSymbol: String, handler: SCNBindingBlock?)

Specifies a block to be called after rendering with programs with the specified GLSL uniform variable or attribute name.

### Constants

typealias SCNBindingBlock

The signature for a block called for binding or unbinding a GLSL symbol in a custom program.

struct SCNShaderModifierEntryPoint

Keys for the shaderModifiers dictionary, each corresponding to an entry point in SceneKit’s shader programs where you can attach a custom GPU shader code snippet.

### Instance Properties

var minimumLanguageVersion: NSNumber?

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- SCNBox
- SCNCapsule
- SCNCone
- SCNCylinder
- SCNFloor
- SCNGeometry
- SCNMaterial
- SCNPlane
- SCNPyramid
- SCNShape
- SCNSphere
- SCNText
- SCNTorus
- SCNTube

## See Also

### Renderer Customization

class SCNProgram

A complete Metal or OpenGL shader program that replaces SceneKit’s rendering of a geometry or material.

protocol SCNBufferStream

An object that manages a Metal buffer used by a custom shader program.

class SCNTechnique

A specification for augmenting or postprocessing SceneKit’s rendering of a scene using additional drawing passes with custom Metal or OpenGL shaders.

protocol SCNTechniqueSupport

The common interface for SceneKit objects that support multipass rendering using SCNTechnique objects.

protocol SCNNodeRendererDelegate

Methods you can implement to use your own custom Metal or OpenGL drawing code to render content for a node.

Postprocessing a Scene With Custom Symbols

Create visual effects in a scene by defining a rendering technique with custom symbols.

