

- SceneKit
- SCNProgram
-  geometryShader 

Instance Property

# geometryShader

GLSL source code for the program’s optional geometry shader.

macOS 10.10+

``` source
var geometryShader: String? { get set }
```

## Discussion

A program’s geometry shader executes once for each geometric primitive (line or triangle) to be rendered. The geometry shader takes as input the vertex positions output by the vertex shader (or by the tessellation shader, if one is in use), and outputs new geometric primitives for rendering.

Geometry shaders require macOS and OpenGL Core Profile. To use OpenGL Core Profile in a SceneKit view, set the view’s pixelFormat property. Geometry shading is optional—to render without a geometry shader, set this property’s value to `nil` (the default).

SceneKit compiles and links your shader program only when it is needed for rendering. To be notified of program compilation errors, provide a delegate object for the program.

## See Also

### Working with OpenGL Shader Source Code

var vertexShader: String?

GLSL source code for the program’s vertex shader.

var fragmentShader: String?

GLSL source code for the program’s fragment shader.

var tessellationControlShader: String?

GLSL source code for the program’s optional tessellation control shader.

var tessellationEvaluationShader: String?

GLSL source code for the program’s optional tessellation evaluation shader.

