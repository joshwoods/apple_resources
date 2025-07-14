

- SceneKit
- SCNProgram
-  delegate 

Instance Property

# delegate

The delegate of the program object.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
unowned(unsafe) var delegate: (any SCNProgramDelegate)? { get set }
```

## Discussion

An SCNProgram object sends delegate messages if errors occur when compiling GLSL source code.

## See Also

### Providing a Delegate Object

protocol SCNProgramDelegate

The interface for tracking errors that occur when compiling shader source code.

