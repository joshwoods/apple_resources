

- SceneKit
- SCNMaterial
-  fillMode 

Instance Property

# fillMode

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var fillMode: SCNFillMode { get set }
```

## See Also

### Customizing Rendered Appearance

var isLitPerPixel: Bool

A Boolean value that determines whether SceneKit performs lighting calculations per vertex or per pixel. Animatable.

var isDoubleSided: Bool

A Boolean value that determines whether SceneKit renders both front and back faces of a surface.

var cullMode: SCNCullMode

The mode determining which faces of a surface SceneKit renders. Animatable.

enum SCNCullMode

The modes SceneKit uses to determine which polygons to render in a surface, used by the cullMode property.

enum SCNFillMode

