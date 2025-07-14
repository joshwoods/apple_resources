

- SceneKit
-  SCNProgram 

Class

# SCNProgram

A complete Metal or OpenGL shader program that replaces SceneKit’s rendering of a geometry or material.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
class SCNProgram
```

## Overview

You use an SCNProgram object to perform custom rendering using shader programs written in the Metal shading language or the OpenGL Shading Language (GLSL). A program object contains a vertex shader and a fragment shader. To use a program object for rendering, assign it to the program property of a geometry or material.

Use a program object when you want to completely replace SceneKit’s rendering. Your shaders take input from SceneKit and become responsible for all transform, lighting, and shading effects that you want to produce.

Note

If instead you want to simply modify or extend SceneKit’s rendering, use the shaderModifiers property of a geometry or material to insert snippets of Metal or GLSL source code into SceneKit’s built-in shader programs. For details on creating and using shader modifiers, see SCNShadable.

To use a custom shader program in SceneKit, create an SCNProgram object and optionally specify its delegate object for handling errors. Next, provide shaders:

- To provide precompiled Metal shader functions, set the vertexFunctionName and fragmentFunctionName properties. SceneKit loads the functions from a Metal shader library in your app’s bundle resources.

- To provide OpenGL or OpenGL ES shader source code, set the vertexShader and fragmentShader properties.

Finally, assign your program object to the geometries or materials you want rendered using the shader program.

Rendering with Metal shaders requires that the renderingAPI property of your SCNView object (or other renderer) be set to SCNRenderingAPI.metal, which in turn requires that your app be running on Metal-capable hardware. If you provide both Metal and OpenGL shaders in the same SCNProgram object, SceneKit automatically selects the appropriate shaders to use when rendering, falling back to OpenGL or OpenGL ES shaders when Metal is not supported on the current hardware.

### Providing Input to a Metal Shader

Metal shaders for use with SceneKit require an `#include ` directive to gain access to SceneKit-specific symbols. Use these symbols to access the kinds of data listed below.

#### Vertex Attributes

To use vertex attributes provided by SCNGeometry objects in your shader program, declare those attributes in your Metal shader source code using attribute qualifiers (see Attribute Qualifiers to Locate Per-Vertex Inputs in Metal Shading Language Guide) and the constants listed in Table 1. For example, the partial shader below declares an input structure using the vertex position and normal attributes.

```
#include 
using namespace metal;
#include 
typedef struct {
    float3 position [[ attribute(SCNVertexSemanticPosition) ]];
    float3 normal   [[ attribute(SCNVertexSemanticNormal) ]];
} MyVertexInput;
```

| Metal Constant | Definition |
|----|----|
| SCNVertexSemanticPosition | The vertex position, provided by the geometry source for the vertex semantic. |
| SCNVertexSemanticNormal | The surface normal vector at the vertex, provided by the geometry source for the normal semantic. |
| SCNVertexSemanticTangent | The surface-space tangent vector.  SceneKit automatically infers this vector based on texture coordinates. To obtain a bitangent vector, take the cross product of the tangent vector and the surface normal vector, and scale the result by the w component of the tangent vector. |
| SCNVertexSemanticColor | The vertex color, provided by the geometry source for the color semantic. |
| SCNVertexSemanticSkinJoints | Skeletal animation index information, provided by the geometry source for the boneIndices semantic. |
| SCNVertexSemanticSkinWeights | Skeletal animation weight information, provided by the geometry source for the boneWeights semantic. |
| SCNVertexSemanticTexcoord0 | Texture coordinates, provided by the first geometry source for the texcoord semantic. |
| SCNVertexSemanticTexcoord1 | Texture coordinates, provided by the second geometry source for the texcoord semantic. |
| SCNVertexSemanticTexcoord2 | Texture coordinates, provided by the third geometry source for the texcoord semantic. |
| SCNVertexSemanticTexcoord3 | Texture coordinates, provided by the fourth geometry source for the texcoord semantic. |

#### Frame-Constant Data

To use information from SceneKit that is constant for all invocations of your shader when rendering a single frame—such as view and projection matrices, fog parameters, and scene time—declare a parameter to your shader function whose type is `SCNSceneBuffer`, with an attribute qualifier binding it to buffer zero. For example, the shader function declaration below uses scene data in its second parameter.

```
vertex MyVertexOutput myVertex(MyVertexInput in [[ stage_in ]],
                                constant SCNSceneBuffer& scn_frame [[buffer(0)]],
                                constant default_node_t& scn_node [[buffer(1)]])
```

Your function can then access scene data from the fields in the `SCNSceneBuffer` structure, outlined below.

```
struct SCNSceneBuffer {
    float4x4    viewTransform;
    float4x4    inverseViewTransform; // view space to world space
    float4x4    projectionTransform;
    float4x4    viewProjectionTransform;
    float4x4    viewToCubeTransform; // view space to cube texture space (right-handed, y-axis-up)
    float4      ambientLightingColor;
    float4      fogColor;
    float3      fogParameters; // x: -1/(end-start) y: 1-start*x z: exponent
    float       time;     // system time elapsed since first render with this shader
    float       sinTime;  // precalculated sin(time)
    float       cosTime;  // precalculated cos(time)
    float       random01; // random value between 0.0 and 1.0
};
```

#### Per-Node Data

To use information from SceneKit that varies for each object being rendered with a shader—such as model and normal matrices—declare a parameter to your shader function with an attribute qualifier binding it to buffer one. For the type of this parameter, declare your own struct type containing any of the fields in Listing 4.

Listing 4. Available Fields for Per-Node Shader Data

```
float4x4 modelTransform;
float4x4 inverseModelTransform;
float4x4 modelViewTransform;
float4x4 inverseModelViewTransform;
float4x4 normalTransform; // Inverse transpose of modelViewTransform
float4x4 modelViewProjectionTransform;
float4x4 inverseModelViewProjectionTransform;
float2x3 boundingBox;
float2x3 worldBoundingBox;
```

For example, the partial shader below declares a struct with model and model-view-projection matrices and uses it in a vertex function.

```
struct MyNodeBuffer {
    float4x4 modelTransform;
    float4x4 modelViewProjectionTransform;
};

vertex MyVertexOutput myVertex(MyVertexInput in [[ stage_in ]],
                                constant SCNSceneBuffer& scn_frame [[buffer(0)]],
                                constant MyNodeBuffer& scn_node [[buffer(1)]])
```

#### Custom Variables

To use custom input variables in a Metal shader, first declare those variables as input parameters to your Metal shader functions, using an attribute qualifier to bind to buffer 2 (or higher). Because these variables pass to your Metal shader in a buffer, you typically also define a data structure for your variables, as seen in the partial shader below.

```
struct MyAccentColors {
    float4 primaryColor;
    float4 secondaryColor;
};

fragment half4 myFragmentShader(default_io in [[stage_in]],
                            constant MyAccentColors& colors [[buffer(2)]]) { ... }
```

There are two options for providing data for your custom variables: manually and at render time.

- To make a single change to your custom variable data, use Key-value coding: Call the setValue(_:forKey:) method on the geometry or material to be rendered with your shader, passing an NSData object containing your data structure as the value and the name of the corresponding shader function parameter as the key. Be aware of layout and alignment when encoding an entire structure as an NSData object—for best results, use data types from the SIMD library (such as `vector_float4` and `matrix_float4x4`), because those types match the layout and alignment of the GPU data types used in a Metal shader.

You can also animate such a change by calling the setValue(_:forKey:) method within an SCNTransaction animation or by creating a CAAnimation object whose key is the shader function parameter name.

In either case, you can alternatively provide a value for a specific member of a structure by wrapping that value in an NSValue object and using the fully qualified name of that member as the key. For example, use `colors.primaryColor` as the key in the example above.

- To update custom variable data at render time, call the handleBinding(ofBufferNamed:frequency:handler:) method to register a block that SceneKit calls before rendering using your shader program. In the block, SceneKit provides an SCNBufferStream object, whose writeBytes(_:count:) you can call to provide a new value for your data structure.

### Providing Input to an OpenGL Shader

Vertex attributes. To use vertex attributes provided by SCNGeometry objects in your shader program, map SceneKit semantics to the input vertex attribute names declared in the shader. Use the setSemantic(_:forSymbol:options:) method and the constants listed in Geometry Semantic Identifiers.

Coordinate transformations. To use the coordinate transformations defined by the scene’s node hierarchy and point-of-view camera in your shader program, map SceneKit’s transform matrices to the uniform variable names declared in the shader. Use the setSemantic(_:forSymbol:options:) method and the constants listed in Rendering Transform Keys.

Custom uniform variables. To provide values for your own custom uniform variables declared in the shader, choose when and how you want to update these values.

- To update a value once, use Key-value coding: Call the setValue(_:forKey:) method, providing the uniform name from shader source code as the key and an appropriate type of data as the value. To smoothly transition a one-time value change, call the setValue(_:forKey:) method inside an SCNTransaction animation or create an animation object with the init(keyPath:) method, passing the uniform name as the key.

- To update a value every time SceneKit renders an object with your shader program, assign binding blocks using the handleBinding(ofSymbol:handler:) method of the geometry or material to be rendered with your custom program. Within a binding block you can execute OpenGL commands to bind shader uniforms or set any other state necessary for rendering.

## Topics

### Working with OpenGL Shader Source Code

var vertexShader: String?

GLSL source code for the program’s vertex shader.

var fragmentShader: String?

GLSL source code for the program’s fragment shader.

var geometryShader: String?

GLSL source code for the program’s optional geometry shader.

var tessellationControlShader: String?

GLSL source code for the program’s optional tessellation control shader.

var tessellationEvaluationShader: String?

GLSL source code for the program’s optional tessellation evaluation shader.

### Mapping GLSL Symbols to SceneKit Semantics

func setSemantic(String?, forSymbol: String, options: [String : Any]?)

Associates a SceneKit semantic identifier with the specified GLSL vertex attribute or uniform variable.

let SCNProgramMappingChannelKey: String

The mapping channel to be used for a texture coordinate semantic.

func semantic(forSymbol: String) -> String?

Returns the SceneKit semantic identifiers associated with the specified GLSL vertex attribute or uniform variable.

let SCNModelTransform: String

A 4 x 4 matrix for transforming coordinates from model space to scene (or world) space.

let SCNModelViewProjectionTransform: String

A 4 x 4 matrix containing the concatenation of the Model, View, and Projection transformations.

let SCNModelViewTransform: String

A 4 x 4 matrix containing the concatenation of the Model and View transformations.

let SCNNormalTransform: String

A 4 x 4 matrix for transforming surface normal vectors from model space to view (or eye) space.

let SCNProjectionTransform: String

A 4 x 4 matrix for transforming coordinates from view (or eye) space to clip space.

let SCNViewTransform: String

A 4 x 4 matrix for transforming coordinates from scene (or world) space to view (or eye) space.

### Providing a Delegate Object

var delegate: (any SCNProgramDelegate)?

The delegate of the program object.

protocol SCNProgramDelegate

The interface for tracking errors that occur when compiling shader source code.

### Managing Opacity

var isOpaque: Bool

A Boolean value that indicates whether fragments rendered by the program are fully opaque.

### Providing Input for Metal Shaders

func handleBinding(ofBufferNamed: String, frequency: SCNBufferFrequency, handler: SCNBufferBindingBlock)

Registers a block for SceneKit to call at render time for binding a Metal buffer to the shader program.

enum SCNBufferFrequency

Options for how often SceneKit should execute the binding handler you provide with the handleBinding(ofBufferNamed:frequency:handler:) method.

typealias SCNBufferBindingBlock

A block SceneKit calls at render time for working with buffers in a Metal shader, used by the handleBinding(ofBufferNamed:frequency:handler:) method.

### Working With Metal Shaders

var vertexFunctionName: String?

The name of the vertex shader function to load from a Metal shader library.

var fragmentFunctionName: String?

The name of the fragment shader function to load from a Metal shader library.

var library: (any MTLLibrary)?

The Metal shader library containing shader functions to be used by this program.

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

## See Also

### Renderer Customization

protocol SCNShadable

Methods for customizing SceneKit’s rendering of geometry and materials using Metal or OpenGL shader programs.

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

