

- Core Animation
- CALayer
-  draw(in:) 

Instance Method

# draw(in:)

Draws the layer’s content using the specified graphics context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func draw(in ctx: CGContext)
```

## Parameters 

`ctx`  

The graphics context in which to draw the content. The context may be clipped to protect valid layer content. Subclasses that wish to find the actual region to draw can call boundingBoxOfClipPath.

## Discussion

The default implementation of this method does not do any drawing itself. If the layer’s delegate implements the draw(_:in:) method, that method is called to do the actual drawing.

Subclasses can override this method and use it to draw the layer’s content. When drawing, all coordinates should be specified in points in the logical coordinate space.

## See Also

### Providing the Layer’s Content

var contents: Any?

An object that provides the contents of the layer. Animatable.

var contentsRect: CGRect

The rectangle, in the unit coordinate space, that defines the portion of the layer’s contents that should be used. Animatable.

var contentsCenter: CGRect

The rectangle that defines how the layer contents are scaled if the layer’s contents are resized. Animatable.

func display()

Reloads the content of this layer.

