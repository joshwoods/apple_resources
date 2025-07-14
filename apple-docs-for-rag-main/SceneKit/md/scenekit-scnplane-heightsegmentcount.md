

- SceneKit
- SCNPlane
-  heightSegmentCount 

Instance Property

# heightSegmentCount

The number of subdivisions in the plane’s surface along its vertical axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var heightSegmentCount: Int { get set }
```

## Discussion

A larger number of segments adds more vertex data to the geometry. Although the plane is flat, extra vertices can be useful for lighting or other special effects. For example, you can add a GLSL source code snippet to the plane’s shaderModifiers property that modulates the position of each vertex. Adding vertices increases rendering cost, so use the minimal segment count that produces your desired visual effect.

The default segment count is `1`. Setting this property’s value to a number less than `1` results in undefined behavior. If the cornerRadius property’s value is greater than zero, the segment count applies to the area between corners.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var cornerSegmentCount: Int

The number of line segments used to create each rounded corner of the plane. Animatable.

### Adjusting Geometric Detail

var widthSegmentCount: Int

The number of subdivisions in the plane’s surface along its horizontal axis. Animatable.

