

- SceneKit
- SCNTechnique
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the value associated with the specified GLSL uniform variable or attribute name, using subscript syntax.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
subscript(key: Any) -> Any? { get }
```

## Parameters 

`key`  

A shader variable or attribute name used in one of the technique’s shader programs.

## Return Value

An object containing the value of the shader symbol.

## Discussion

This method returns an object appropriate to the type of the shader symbol being set. For example, retrieving the value of a `float` uniform variable returns an NSNumber object, and retrieving the value of a GLSL `vec3` uniform variable or Metal `float3` variable returns an NSValue object containing an SCNVector3 structure.

## See Also

### Handling Parameters for a Technique’s Shader Programs

func handleBinding(ofSymbol: String, using: SCNBindingBlock?)

Specifies a block to be called before rendering using programs with the specified GLSL uniform variable or attribute name.

func setObject(Any?, forKeyedSubscript: any NSCopying)

Sets a value for the specified shader variable or attribute name, using subscript syntax.

