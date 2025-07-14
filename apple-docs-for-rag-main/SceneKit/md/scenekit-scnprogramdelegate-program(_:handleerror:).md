

- SceneKit
- SCNProgramDelegate
-  program(\_:handleError:) 

Instance Method

# program(\_:handleError:)

Tells the delegate that an error occurred when compiling GLSL source code.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
optional func program(
    _ program: SCNProgram,
    handleError error: any Error
)
```

## Parameters 

`program`  

The program that generated the compilation error.

`error`  

The compilation error that was raised.

## Discussion

Examine the `error` parameter for details of the compilation error provided by the GLSL compiler.

## See Also

### Handling Shader Compilation Errors

let SCNErrorDomain: String

Identifies an error type defined by the SceneKit framework.

SceneKit Error Codes

