

- SceneKit
- SCNProgramDelegate
-  program(\_:bindValueForSymbol:atLocation:programID:renderer:) Deprecated

Instance Method

# program(\_:bindValueForSymbol:atLocation:programID:renderer:)

Invoked on the delegate to let it bind program values and/or associated graphics resources (such as textures) for symbols.

macOS 10.8–10.10Deprecated

``` source
optional func program(
    _ program: SCNProgram,
    bindValueForSymbol symbol: String,
    atLocation location: UInt32,
    programID: UInt32,
    renderer: SCNRenderer
) -> Bool
```

Deprecated

Use the handleBinding(ofSymbol:handler:) method of the geometry or material the program is attached to.

## Parameters 

`program`  

The `SCNProgram` object to bind values for.

`symbol`  

The name of the symbol to bind a value for.

`location`  

The location of the symbol within the program object to be modified.

`programID`  

The underlying OpenGL program object in which the binding is made.

`renderer`  

The renderer that is currently rendering the scene.

## Discussion

If you use the handleBinding(ofSymbol:handler:) method to associate a handler block with a SceneKit object for a symbol, SceneKit will not call the delegate’s program(_:bindValueForSymbol:atLocation:programID:renderer:) method for that symbol when rendering that object.

## See Also

### Binding and Unbinding Values

func program(SCNProgram, unbindValueForSymbol: String, atLocation: UInt32, programID: UInt32, renderer: SCNRenderer)

Invoked on the delegate to let it unbind program values and/or also unbind associated graphic resources (such as textures).

Deprecated

