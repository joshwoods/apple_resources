

- Core Animation
- CALayer
-  contentsRect 

Instance Property

# contentsRect

The rectangle, in the unit coordinate space, that defines the portion of the layer’s contents that should be used. Animatable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
var contentsRect: CGRect { get set }
```

## Discussion

Defaults to the unit rectangle (0.0, 0.0, 1.0, 1.0).

If pixels outside the unit rectangle are requested, the edge pixels of the contents image will be extended outwards.

If an empty rectangle is provided, the results are undefined.

## See Also

### Providing the Layer’s Content

var contents: Any?

An object that provides the contents of the layer. Animatable.

var contentsCenter: CGRect

The rectangle that defines how the layer contents are scaled if the layer’s contents are resized. Animatable.

func display()

Reloads the content of this layer.

func draw(in: CGContext)

Draws the layer’s content using the specified graphics context.

