

- SceneKit
- SCNShadable
-  handleUnbinding(ofSymbol:handler:) 

Instance Method

# handleUnbinding(ofSymbol:handler:)

Specifies a block to be called after rendering with programs with the specified GLSL uniform variable or attribute name.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOS

``` source
optional func handleUnbinding(
    ofSymbol symbol: String,
    handler block: SCNBindingBlock? = nil
)
```

## Parameters 

`symbol`  

A GLSL uniform variable or attribute name.

`block`  

A block to be called by SceneKit.

## Discussion

Use this method to associate a block with a SceneKit object (geometry or material) to handle cleanup related to an attribute or uniform variable in a custom SCNProgram shader associated with that object. SceneKit will call your block after rendering the object. In the block, you can execute any OpenGL commands or other code necessary for post-rendering tasks.

This method is for OpenGL shader programs only. To bind custom variable data for Metal shader programs, use the handleBinding(ofBufferNamed:frequency:handler:) method.

## See Also

### Handling Parameters in Custom OpenGL Shader Programs

func handleBinding(ofSymbol: String, handler: SCNBindingBlock?)

Specifies a block to be called before rendering with programs with the specified GLSL uniform variable or attribute name.

