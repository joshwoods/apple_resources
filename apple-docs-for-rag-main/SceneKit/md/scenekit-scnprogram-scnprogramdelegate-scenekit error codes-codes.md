

- SceneKit
- SCNProgram
- SCNProgramDelegate
-  SceneKit Error Codes 

API Collection

# SceneKit Error Codes

## Discussion

Constants for the code property of NSError objects produced by the SceneKit framework.

## Topics

### Constants

var SCNProgramCompilationError: Int

An error in compiling GLSL shader source code for use with the SCNProgram class.

## See Also

### Handling Shader Compilation Errors

func program(SCNProgram, handleError: any Error)

Tells the delegate that an error occurred when compiling GLSL source code.

let SCNErrorDomain: String

Identifies an error type defined by the SceneKit framework.

