

- SceneKit
- SCNTechnique
-  handleBinding(ofSymbol:using:) 

Instance Method

# handleBinding(ofSymbol:using:)

Specifies a block to be called before rendering using programs with the specified GLSL uniform variable or attribute name.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func handleBinding(
    ofSymbol symbol: String,
    using block: SCNBindingBlock? = nil
)
```

## Parameters 

`symbol`  

A GLSL uniform variable or attribute name used in one of the technique’s shader programs.

`block`  

A block that SceneKit calls.

## Discussion

This method associates a block for handling setup of an attribute or uniform variable in the shader programs associated with the technique. SceneKit calls your block before any performing any rendering passes that use that symbol. In the block, you can execute any OpenGL commands or other code necessary for preparing your custom shader.

Note

You must associate a handler block with a technique before assigning that technique to a SceneKit object. The result of calling this method on a technique currently in use is undefined.

Use this method when you need to update a value in a shader program every time SceneKit renders a frame. To set a value infrequently, or only once, use the setObject(_:forKeyedSubscript:) or setValue(_:forKey:) method instead.

If you associate a block with a symbol using this method, SceneKit ignores values set using the setObject(_:forKeyedSubscript:) method.

## See Also

### Handling Parameters for a Technique’s Shader Programs

func setObject(Any?, forKeyedSubscript: any NSCopying)

Sets a value for the specified shader variable or attribute name, using subscript syntax.

subscript(Any) -> Any?

Returns the value associated with the specified GLSL uniform variable or attribute name, using subscript syntax.

