

- SceneKit
- SCNProgram
-  tessellationControlShader 

Instance Property

# tessellationControlShader

GLSL source code for the program’s optional tessellation control shader.

macOS 10.10+

``` source
var tessellationControlShader: String? { get set }
```

## Discussion

A program’s tessellation control shader executes once for each vertex in the geometry it renders. The tessellation control shader takes as input the vertex positions output by the vertex shader, and outputs tessellation-level information to be used by the hardware tessellator for subdividing polygons and edges. The tessellator then provides input to your tessellation evaluation shader.

Tessellation shaders require macOS and OpenGL Core Profile. To use OpenGL Core Profile in a SceneKit view, set the view’s pixelFormat property. Tessellation shading is optional—to render without a tessellation shader, set this property’s value to `nil` (the default). However, if you specify a tessellation control shader, a tessellation evaluation shader is also required.

SceneKit compiles and links your shader program only when it is needed for rendering. To be notified of program compilation errors, provide a delegate object for the program.

## See Also

### Working with OpenGL Shader Source Code

var vertexShader: String?

GLSL source code for the program’s vertex shader.

var fragmentShader: String?

GLSL source code for the program’s fragment shader.

var geometryShader: String?

GLSL source code for the program’s optional geometry shader.

var tessellationEvaluationShader: String?

GLSL source code for the program’s optional tessellation evaluation shader.

