

- RealityKit
- CustomMaterial
-  writesDepth 

Instance Property

# writesDepth

A boolean value that determines whether this material writes its depth into RealityKit’s depth buffer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var writesDepth: Bool { get set }
```

## Discussion

If true, meshes with this material will occlude objects behind them by writing their depth into RealityKit’s depth buffer.

If false, meshes with this material will not write their depth into RealityKit’s depth buffer, and may be overwritten by objects drawn behind them, depending on draw order.

The default value is true.

## See Also

### Setting depth testing properties

var readsDepth: Bool

A boolean value that determines whether this material performs the depth test by reading RealityKit’s depth buffer.

