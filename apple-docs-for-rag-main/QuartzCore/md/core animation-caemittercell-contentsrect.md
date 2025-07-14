

- Core Animation
- CAEmitterCell
-  contentsRect 

Instance Property

# contentsRect

A rectangle (in the unit coordinate space) that specifies the portion of contents that the receiver should draw. Animatable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
var contentsRect: CGRect { get set }
```

## Discussion

By default, this property is set to the unit rectangle (0.0,0.0,1.0,1.0), which results in all of the layer’s contents being drawn.

If pixels outside the unit rectangle are requested, the edge pixels of the contents image are extended outwards.

If you assign an empty rectangle to this property, the results are undefined.

## See Also

### Providing Emitter Cell Content

var contents: Any?

An object that provides the contents of the layer. Animatable.

var emitterCells: [CAEmitterCell]?

An optional array containing the sub-cells of this cell.

