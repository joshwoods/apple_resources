

- SceneKit
-  SCNTechnique 

Class

# SCNTechnique

A specification for augmenting or postprocessing SceneKit’s rendering of a scene using additional drawing passes with custom Metal or OpenGL shaders.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNTechnique
```

## Overview

Examples of multipass rendering techniques include:

- Postprocessing rendered pixels. To create effects such as color grading and displacement mapping, define techniques that use as input the color buffer rendered by SceneKit and process that buffer with a fragment shader.

- Deferred shading. To create effects such as motion blur and screen-space ambient occlusion (SSAO), define techniques that capture information about the scene into an intermediary buffer during the main rendering pass and then perform additional drawing passes using that buffer to create the final output image. The figure below illustrates the rendering process for an SSAO technique.

To create an SCNTechnique object, you supply a technique definition that specifies the input and output image buffers, shader programs, shader input variables, and rendering options for each drawing pass in the technique. Defining a technique does not require Metal or OpenGL client code, but you should be familiar with the terminology and conventions of GPU rendering.

To use a technique, assign it to the technique property of a view (or other SceneKit renderer object) or a camera.

### Defining a Technique

SceneKit treats rendering techniques—along with shaders, 3D models, and 2D art assets—as resources rather than as part of your application code. Because the effects you create with techniques are highly visual, this approach allows you to separate design efforts from development efforts and quickly iterate on creating the visual content of your app or game.

Create a technique object using the init(dictionary:) method, providing a dictionary that defines the technique as a series of drawing passes, each with its own shader program, inputs and outputs, and rendering options. Typically, you obtain this dictionary from a property list file included in your app’s bundle resources. Table 1 and the additional tables and sections that follow specify the format of this dictionary’s contents.

| Key | Value |
|----|----|
| `passes` | A dictionary of drawing pass definitions.  Each key is a unique string you provide to identify the pass, and the corresponding value is a dictionary defining that drawing pass. See Table 2. |
| `sequence` | An array of strings, each of which names a drawing pass from the `passes` dictionary. SceneKit performs the drawing passes in the order specified by this array. |
| `symbols` | A dictionary defining the bindings for GLSL attributes and uniform variables used in the technique’s shader programs.  Each key matches the name of a symbol used in the shader source code, and the corresponding value is a dictionary describing how that symbol should be used. See Table 4. |
| `targets` (optional) | A dictionary defining intermediary rendering targets.  Each key is a unique string you provide to identify the target (used in the inputs and outputs dictionaries of a drawing pass definition), and the corresponding value is a dictionary defining the rendering target. See Table 5. |

| Key | Type | Value |
|----|----|----|
| `draw` | String | What to render for the drawing pass:  `DRAW_SCENE`: Render the entire scene.  `DRAW_NODE`: Render only the node specified by the `node` key (and its hierarchy of child nodes).  `DRAW_QUAD`: Render only a rectangle covering the entire bounds of the view. Use this option for drawing passes that process image buffers output by earlier passes. |
| `program` | String | The GLSL shader program to use for the drawing pass.  Shader source code files in the app’s bundle resources directory must have the same base name and the extensions `.vsh` (vertex shader) and `.fsh` (fragment shader). For example, if the program name is “invert”, the files “invert.fsh” and “invert.vsh” must exist. |
| `metalVertexShader`  `metalFragmentShader` | String | The names of the Metal vertex and fragment shader functions to use for the drawing pass. These functions must exist in the app’s default Metal library.  You must specify both fragment and vertex shaders, and you must specify either a GLSL shader program, a pair of Metal functions, or both. If both are specified, SceneKit uses whichever shader is appropriate for the current renderer. |
| `inputs` | Dictionary | Definitions of input variables for the drawing pass.  Each key is the name of a uniform variable used in the GLSL shader source code referenced by the program key. The corresponding value may be any of:  A symbol name from the technique’s `symbols` dictionary  A render target name (see Render Targets, Inputs and Outputs)  A dictionary describing a texture sampler (see Table 6) |
| `outputs` | Dictionary | Definitions of output image buffers for the drawing pass.  Each key is one of the strings `color`, `depth`, or `stencil`, and the corresponding value is a string identifying a render target. See Render Targets, Inputs and Outputs. |
| `node` (optional) | String | The name property of the node to render, or `self` to reference the node the technique is attached to. Applies only if the `draw` key specifies `DRAW_NODE`. |
| `colorStates` (optional) | Dictionary | Options for the color output; one or more of these keys and values:  `clear` (Boolean, defaults to false in macOS and true on iOS): Whether to clear the rendering target before drawing. If true, you must specify one of the `clearColor` and `clearWithSceneBackgroundColor` options.  `clearColor` (string): The color to fill the render target with when clearing, specified in floating-point RGBA format. (For example, “0.5 0.5 0.5 1.0” is a fully opaque gray color.) Alternatively, the string `sceneBackground` specifies to use the scene’s background property when clearing. |
| `depthStates` (optional) | Dictionary | Options for the depth output; one or more of these keys and values:  `clear` (Boolean, default false): Whether to clear the depth buffer before drawing.  `enableWrite` (Boolean, default true): Whether to write to the depth buffer when drawing.  `enableRead` (Boolean, default true): Whether to read from the depth buffer when drawing.  `func` (string): The depth test function: `never`, `always`, `equal`, `notEqual`, `less`, `lessEqual`, `greater`, or `greaterEqual`. |
| `stencilStates` (optional) | Dictionary | Options for the stencil output; one or more of these keys and values:  `clear` (Boolean, default false): Whether to clear the stencil buffer before drawing.  `enable` (Boolean, default false): Whether the drawing pass should write to the stencil buffer.  `behavior`: A dictionary specifying how to use the stencil buffer when rendering front faces (or both faces, if nothing is specified for the `backFaceBehavior` key). See Table 3.  `backFaceBehavior`: A dictionary specifying how to use the stencil buffer when rendering back faces. See Table 3. |
| `cullMode` (optional) | String | The faces of scene geometry to be rendered:  `back` (default): Cull back faces, rendering front faces only.  `front`: Cull front faces, rendering back faces only.  `none`: Render both front- and back-facing polygons. |
| `blendStates` (optional) | Dictionary | Options for color blending; one or more of these keys and values:  `enable` (Boolean): Whether to use color blending. If false, the other blending options have no effect.  `colorSrc` (string): The blend mode for source colors.  `colorDst` (string): The blend mode for destination colors.  `alphaSrc` (string): The blend mode for source alpha values.  `alphaDst` (string): The blend mode for destination alpha values.  `colorOp` (string): The blend operation for color components.  `alphaOp` (string): The blend operation for alpha values.  See Blending. |
| `viewport` (optional) | String | A custom viewport rectangle in view coordinates, formatted as four numbers (origin x, origin y, width, and height). By default, a drawing pass covers the entire bounds of the view. |
| `pointOfView` (optional) | String | The name of a node in the scene to use as the viewer’s position for rendering; equivalent to the pointOfView property on a renderer. |
| `samples` (optional) | Number (unsigned integer) | The number of samples per pixel for enabling multisampled rendering for the drawing pass. Defaults to `1`. |
| `includeCategoryMask` (optional) | Number (8-bit unsigned integer) | A bitfield used for including nodes in the drawing pass if the `draw` key specifies `DRAW_SCENE` or `DRAW_NODE`. Defaults to all bits set. See Category Masks. |
| `excludeCategoryMask` (optional) | Number (8-bit unsigned integer) | A bitfield used for excluding nodes from the drawing pass if the `draw` key specifies `DRAW_SCENE` or `DRAW_NODE`. Defaults to no bits set. See Category Masks. |

| Key | Type | Value |
|----|----|----|
| `depthFail` | String | The stencil operation to use if the depth test fails: `keep`, `zero`, `replace`, `increment`, `decrement`, `invert`, `incrementWrap`, or `decrementWrap`. |
| `fail` | String | The stencil operation to use if the depth test succeeds and the stencil test fails: `keep`, `zero`, `replace`, `increment`, `decrement`, `invert`, `incrementWrap`, or `decrementWrap`. |
| `pass` | String | The stencil operation to use if the depth and stencil tests succeed: `keep`, `zero`, `replace`, `increment`, `decrement`, `invert`, `incrementWrap`, or `decrementWrap`. |
| `function` | String | The stencil test function: `never`, `always`, `equal`, `notEqual`, `less`, `lessEqual`, `greater`, or `greaterEqual`. |
| `readMask` | Number (8-bit unsigned integer) | A bitmask for selecting the bit plane of the stencil buffer to be tested. |
| `writeMask` | Number (8-bit unsigned integer) | A bitmask for selecting the bit plane of the stencil buffer to write to. |
| `referenceValue` | Number (8-bit unsigned integer) | The reference value for stencil tests. Defaults to `0`. |

| Key | Type | Value |
|----|----|----|
| `semantic` | String | Use this option to bind shader symbols to data supplied by SceneKit:  The values `vertex`, `normal`, `color`, and `texcoord` bind to geometry source semantics. See Geometry Semantic Identifiers.  The values `modelViewProjectionTransform`, `modelViewTransform`, `modelTransform`, `viewTransform`, `projectionTransform`, `normalTransform`, `modelViewProjectionInverseTransform`, `modelViewInverseTransform`, `modelInverseTransform`, `viewInverseTransform`, `projectionInverseTransform`, and `normalInverseTransform` bind to rendering transformation matrices. See Rendering Transform Keys.  The value `time` binds the system time elapsed since rendering began.  If you set a `semantic` value for a symbol, no `type` value is required. |
| `type` | String | The GLSL type of the input variable: `float`, `vec2`, `vec3`, `vec4`, `mat4`, `int`, `ivec2`, `ivec3`, `ivec4`, `mat3`, `sampler2D`, or `none`.  Use this option when providing custom values to shader programs (see Handling Parameters for a Technique’s Shader Programs). |
| `image` (optional) | String | If the symbol’s type is `sampler2D`, the name of an image file in the app’s bundle resources directory. |

#### Category Masks

When SceneKit performs a rendering pass whose `draw` option is `DRAW_SCENE` or `DRAW_NODE`, you can use category masks to filter the set of nodes drawn during that pass. For each node in the scene (or for `DRAW_NODE`, in the node subtree), SceneKit compares the node’s categoryBitMask property and the `includeCategoryMask` and `excludeCategoryMask` options in the pass definition using bitwise AND operations. If the node’s category mask and the include mask overlap (that is, the bitwise AND results in a nonzero value) and the node’s category mask and the exclude mask do not overlap, SceneKit includes the node in the drawing pass. Otherwise the node is not rendered in the pass.

#### Render Targets, Inputs and Outputs

A drawing pass renders pixel data into one or more target image buffer (or framebuffer). In SceneKit’s main drawing pass, the color render target is the screen (or rather, a view or layer for screen display), and a depth render target temporarily stores the information needed to ensure that rendered surfaces appear in the correct depth order.

A pass in a custom rendering technique may postprocess the pixel data in SceneKit’s render target, generate its own pixel data for display, or render to an intermediate target to be used as input in a later pass. You specify render targets using the following identifiers in the `inputs` and `outputs` dictionaries of a pass definition:

- Use the `COLOR` and `DEPTH` targets as inputs to identify the color and depth buffers rendered to in SceneKit’s main drawing pass.

Use the `COLOR` target as an output to identify the image buffer displayed as the end result of a technique.

- To create an intermediate target, define your own identifier as a key in the `targets` dictionary of a technique definition. For the corresponding value, provide a dictionary defining the render target using the keys and values in Table 5. Intermediate targets may be color, depth, or combined depth and stencil buffers. After you define a target, you can use its identifier in the `inputs` and `outputs` dictionaries of a pass definition.

- To use an image as an input texture for a pass, define a symbol of type `sampler2D` in the technique’s `symbols` dictionary.

To specify a render target or image sampler in the `inputs` dictionary of a pass definition, you can provide either an identifier string or a dictionary with the format described in Table 6. The options for samplers correspond to similar properties for SceneKit material textures. For more details on each, see SCNMaterialProperty.

| Key | Type | Value |
|----|----|----|
| `type` | String | The type of render target: `color`, `depth`, or `stencil`. |
| `format` (optional) | String | The render target’s pixel format; one of the following:  Color: `rgba` (default), `rgb32f`, `r8`, or `r16`  Depth/stencil: `depth24` (default) or `depth24stencil8` |
| `size` | String | The size of the render target image, in points, specified in a string of format “WxH”. For example, the string “320x480” specifies an image buffer 320 points wide by 480 points tall. |
| `scaleFactor` (optional) | Number (floating-point) | The scale factor of the render target. Defaults to `1.0`. For example, a value of `2.0` specifies 2 pixels per point, so a target whose size is “320x480” is 640 by 960 pixels. |

| Key | Type | Value |
|----|----|----|
| `target` | String | `COLOR`, `DEPTH`, a key from the technique’s `targets` dictionary, or a key from the technique’s `symbols` dictionary identifying a texture sampler. |
| `magnificationFilter` (optional)  `minificationFilter` (optional) | String | `linear` or `nearest`. |
| `mipFilter` (optional) | String | `linear`, `nearest`, or `none`. |
| `wrapS` (optional)  `wrapT` (optional)  `wrapP` (optional) | String | `clamp`, `repeat`, `clampToBorder`, `mirror`. |

#### Blending

The `blendStates` key of a pass definition defines color blending options. Blending is disabled by default for faster rendering performance. Including a dictionary for this key enables blending (unless the dictionary’s `enable` key specifies false). Color blending combines a source color (the color output by the drawing pass’s shader program) with a destination color (the existing contents of the output buffer) using specified modes and operations.

- Available blend modes (for the `colorSrc`, `colorDst`, `alphaSrc`, and `alphaDst` keys): `zero`, `one`, `srcColor`, `oneMinusSrcColor`, `srcAlpha`, `oneMinusSrcAlpha`, `dstColor`, `oneMinusDstColor`, `dstAlpha`, `oneMinusDstAlpha`, `constantColor`, `oneMinusConstantColor`, `constantAlpha`, `oneMinusConstantAlpha`, and `alphaSaturate`.

- Available blend operations (for the `colorOp` and `alphaOp` keys): `add`, `subtract`, `reverseSubtract`, `min`, `max`.

These values correspond to blending options defined by the OpenGL specification. For further details, consult the OpenGL API Registry or OpenGL ES API Registry.

### Example Technique Definition

Listing 1 shows an example definition dictionary for a technique that uses displacement mapping with a noise texture to postprocess a rendered scene. For ease of reading, the dictionary is formatted in JSON syntax. (To load an NSDictionary object from text in this format, use the JSONSerialization class.) Listing 2 and Listing 3 show the GLSL source code for the technique’s vertex and fragment shaders.

Listing 1. JSON definition dictionary for a technique

```
{
  "passes" : {
    "displacement" : {
      "outputs" : {
        "color" : "COLOR"
      },
      "inputs" : {
        "colorSampler" : "COLOR",
        "noiseSampler" : "noiseSymbol",
        "a_position" : "a_position-symbol"
      },
      "program" : "displacement",
      "draw" : "DRAW_QUAD"
    }
  },
  "sequence" : [
    "displacement"
  ],
  "symbols" : {
    "a_position-symbol" : {
      "semantic" : "vertex"
    },
    "noiseSymbol" : {
      "image" : "noise.png",
      "type" : "sampler2D"
    }
  }
}
```

Listing 2. GLSL Vertex shader source code for displacement mapping technique

```
attribute vec4 a_position;
varying vec2 uv;

void main() {
    gl_Position = a_position;
    uv = (a_position.xy + 1.0) * 0.5;
}
```

Listing 3. GLSL Fragment shader source code for displacement mapping technique

```
uniform sampler2D colorSampler;
uniform sampler2D noiseSampler;

varying vec2 uv;

void main() {
    vec2 displacement = texture2D(noiseSampler, uv).rg - vec2(0.5, 0.5);
    gl_FragColor = texture2D(colorSampler, uv + displacement * vec2(0.1,0.1));
}
```

## Topics

### Creating a Technique

init?(dictionary: [String : Any])

Creates a technique from a technique definition dictionary.,

### Combining Techniques

init?(bySequencingTechniques: [SCNTechnique])

Creates a new rendering technique that combines a series of techniques.

### Retrieving a Technique’s Definition

var dictionaryRepresentation: [String : Any]

The dictionary defining the rendering technique.

### Handling Parameters for a Technique’s Shader Programs

func handleBinding(ofSymbol: String, using: SCNBindingBlock?)

Specifies a block to be called before rendering using programs with the specified GLSL uniform variable or attribute name.

func setObject(Any?, forKeyedSubscript: any NSCopying)

Sets a value for the specified shader variable or attribute name, using subscript syntax.

subscript(Any) -> Any?

Returns the value associated with the specified GLSL uniform variable or attribute name, using subscript syntax.

### Instance Properties

var library: (any MTLLibrary)?

## Relationships

### Inherits From

- NSObject

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
- SCNAnimatable

## See Also

### Renderer Customization

protocol SCNShadable

Methods for customizing SceneKit’s rendering of geometry and materials using Metal or OpenGL shader programs.

class SCNProgram

A complete Metal or OpenGL shader program that replaces SceneKit’s rendering of a geometry or material.

protocol SCNBufferStream

An object that manages a Metal buffer used by a custom shader program.

protocol SCNTechniqueSupport

The common interface for SceneKit objects that support multipass rendering using SCNTechnique objects.

protocol SCNNodeRendererDelegate

Methods you can implement to use your own custom Metal or OpenGL drawing code to render content for a node.

Postprocessing a Scene With Custom Symbols

Create visual effects in a scene by defining a rendering technique with custom symbols.

