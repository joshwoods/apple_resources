

- SceneKit
- SCNShadable
-  shaderModifiers 

Instance Property

# shaderModifiers

A dictionary of GLSL source code snippets for customizing the shader programs provided by SceneKit.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
optional var shaderModifiers: [SCNShaderModifierEntryPoint : String]? { get set }
```

## Discussion

The dictionary’s keys must be from the set of constants described in `Shader Modifier Entry Point Keys`. Each key represents a possible entry point in SceneKit’s shader programs, whose corresponding value is an NSString object containing a shader source code snippet to be included in the shader program at that entry point.

See Use Shader Modifiers to Extend SceneKit Shading in the protocol overview for a complete discussion of shader modifiers.

