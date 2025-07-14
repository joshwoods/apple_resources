

- SceneKit
- SCNProgram
-  fragmentShader 

Instance Property

# fragmentShader

GLSL source code for the program’s fragment shader.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var fragmentShader: String? { get set }
```

## Discussion

A program’s fragment shader (sometimes called a *pixel shader*) executes at least once for each pixel in rendered output. The fragment shader takes as input the values output by the vertex shader (after those values have been interpolated by the GPU), and uses them to compute a final color for each pixel.

SceneKit compiles and links your shader program only when it is needed for rendering. To be notified of program compilation errors, provide a delegate object for the program.

## See Also

### Working with OpenGL Shader Source Code

var vertexShader: String?

GLSL source code for the program’s vertex shader.

var geometryShader: String?

GLSL source code for the program’s optional geometry shader.

var tessellationControlShader: String?

GLSL source code for the program’s optional tessellation control shader.

var tessellationEvaluationShader: String?

GLSL source code for the program’s optional tessellation evaluation shader.

