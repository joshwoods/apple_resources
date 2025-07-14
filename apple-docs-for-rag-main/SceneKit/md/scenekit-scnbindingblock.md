

- SceneKit
-  SCNBindingBlock 

Type Alias

# SCNBindingBlock

The signature for a block called for binding or unbinding a GLSL symbol in a custom program.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SCNBindingBlock = (UInt32, UInt32, SCNNode?, SCNRenderer) -> Void
```

## Discussion

The block takes the following parameters:

`programID`  
The OpenGL program identifier for the current SCNProgram instance, as used by OpenGL functions such as `glValidateProgram`.

`location`  
The OpenGL location index for the symbol to be bound or unbound, as used by OpenGL functions such as `glUniform`.

`renderedNode`  
The SCNNode object being rendered.

`renderer`  
The SCNRenderer object responsible for rendering.

Call handleBinding(ofSymbol:handler:) or handleUnbinding(ofSymbol:handler:) to associate a handler block with a GLSL symbol for a SceneKit geometry or material.

## See Also

### Constants

struct SCNShaderModifierEntryPoint

Keys for the shaderModifiers dictionary, each corresponding to an entry point in SceneKit’s shader programs where you can attach a custom GPU shader code snippet.

