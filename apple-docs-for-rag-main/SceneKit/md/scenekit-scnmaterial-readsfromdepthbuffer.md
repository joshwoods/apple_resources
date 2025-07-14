

- SceneKit
- SCNMaterial
-  readsFromDepthBuffer 

Instance Property

# readsFromDepthBuffer

A Boolean value that determines whether SceneKit uses depth information when rendering the material.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var readsFromDepthBuffer: Bool { get set }
```

## Discussion

SceneKit’s rendering process uses a depth buffer to determine the ordering of rendered surfaces relative to the viewer. The default value of this property is true, specifying that SceneKit compares the depth of each rendered pixel to the corresponding value in its depth buffer when rendering the material. If the pixel is at a greater depth than the corresponding point in the depth buffer, SceneKit does not render the pixel.

Typically, you disable reading from the depth buffer when rendering objects that should always be visible regardless of the already rendered content in the scene—for example, a heads-up display in a game. In such cases, you should also set a high value for the renderingOrder property of the node containing whatever content is to be always visible.

## See Also

### Managing Render Targets

var writesToDepthBuffer: Bool

A Boolean value that determines whether SceneKit produces depth information when rendering the material.

var colorBufferWriteMask: SCNColorMask

struct SCNColorMask

