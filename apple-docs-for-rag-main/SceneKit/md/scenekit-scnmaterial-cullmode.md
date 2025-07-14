

- SceneKit
- SCNMaterial
-  cullMode 

Instance Property

# cullMode

The mode determining which faces of a surface SceneKit renders. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var cullMode: SCNCullMode { get set }
```

## Discussion

The vertex data and normal vectors in a geometry designate which side of each polygon is to be considered its front face, and the geometry’s orientation with respect to the camera determines which front surfaces are currently visible. Typically, back-facing surfaces are found only on the interior of a closed geometry, obscured by front-facing surfaces, so rendering these surfaces has a performance cost but no visible effect.

This property’s default value is SCNCullBack, specifying that SceneKit should cull, or not render, back-facing surfaces. You can change this property’s value to cause SceneKit to render only the back surfaces of a material instead. See SCNCullMode for available values.

You can animate changes to this property’s value. See Animating SceneKit Content. Animating this property fades between the results of rendering with each state

## See Also

### Customizing Rendered Appearance

var isLitPerPixel: Bool

A Boolean value that determines whether SceneKit performs lighting calculations per vertex or per pixel. Animatable.

var isDoubleSided: Bool

A Boolean value that determines whether SceneKit renders both front and back faces of a surface.

enum SCNCullMode

The modes SceneKit uses to determine which polygons to render in a surface, used by the cullMode property.

var fillMode: SCNFillMode

enum SCNFillMode

