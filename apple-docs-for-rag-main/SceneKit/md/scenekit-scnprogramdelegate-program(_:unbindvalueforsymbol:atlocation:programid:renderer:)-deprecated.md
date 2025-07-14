

- SceneKit
- SCNProgramDelegate
-  program(\_:unbindValueForSymbol:atLocation:programID:renderer:) Deprecated

Instance Method

# program(\_:unbindValueForSymbol:atLocation:programID:renderer:)

Invoked on the delegate to let it unbind program values and/or also unbind associated graphic resources (such as textures).

macOS 10.8–10.10Deprecated

``` source
optional func program(
    _ program: SCNProgram,
    unbindValueForSymbol symbol: String,
    atLocation location: UInt32,
    programID: UInt32,
    renderer: SCNRenderer
)
```

Deprecated

Use the handleUnbinding(ofSymbol:handler:) method of the geometry or material the program is attached to.

## Parameters 

`program`  

The `SCNProgram` object to unbind values for.

`symbol`  

The name of the symbol to unbind a value for.

`location`  

The location of the symbol within the program object to be modified.

`programID`  

The underlying OpenGL program object in which the unbinding is done.

`renderer`  

The renderer that is currently rendering the scene.

## Discussion

If you use the handleUnbinding(ofSymbol:handler:) method to associate a handler block with a SceneKit object for a symbol, SceneKit will not call the delegate’s program(_:unbindValueForSymbol:atLocation:programID:renderer:) method for that symbol when rendering that object.

## See Also

### Binding and Unbinding Values

func program(SCNProgram, bindValueForSymbol: String, atLocation: UInt32, programID: UInt32, renderer: SCNRenderer) -> Bool

Invoked on the delegate to let it bind program values and/or associated graphics resources (such as textures) for symbols.

Deprecated

