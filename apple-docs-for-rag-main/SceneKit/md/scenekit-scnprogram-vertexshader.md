

- SceneKit
- SCNProgram
-  vertexShader 

Instance Property

# vertexShader

GLSL source code for the program’s vertex shader.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var vertexShader: String? { get set }
```

## Discussion

A program’s vertex shader executes once for each vertex in the geometry it renders. It takes as input the attributes of each vertex (such as position in model space, normal vectors, and texture coordinates). The vertex shader then outputs a clip-space position for the vertex, as well as values that the GPU interpolates across a surface and sends to the fragment shader.

SceneKit compiles and links your shader program only when it is needed for rendering. To be notified of program compilation errors, provide a delegate object for the program.

## See Also

### Working with OpenGL Shader Source Code

var fragmentShader: String?

GLSL source code for the program’s fragment shader.

var geometryShader: String?

GLSL source code for the program’s optional geometry shader.

var tessellationControlShader: String?

GLSL source code for the program’s optional tessellation control shader.

var tessellationEvaluationShader: String?

GLSL source code for the program’s optional tessellation evaluation shader.

