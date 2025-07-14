

- SceneKit
- SCNMaterial
-  writesToDepthBuffer 

Instance Property

# writesToDepthBuffer

A Boolean value that determines whether SceneKit produces depth information when rendering the material.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var writesToDepthBuffer: Bool { get set }
```

## Discussion

SceneKit’s rendering process uses a depth buffer to determine the ordering of rendered surfaces relative to the viewer. The default value of this property is true, specifying that SceneKit saves depth information for each rendered pixel for use by later rendering passes.

Typically, you disable writing to the depth buffer when rendering semitransparent objects, because later stages of the rendering process may require depth information about the opaque objects behind them.

## See Also

### Managing Render Targets

var readsFromDepthBuffer: Bool

A Boolean value that determines whether SceneKit uses depth information when rendering the material.

var colorBufferWriteMask: SCNColorMask

struct SCNColorMask

