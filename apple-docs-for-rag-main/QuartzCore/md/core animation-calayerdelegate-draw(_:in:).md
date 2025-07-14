

- Core Animation
- CALayerDelegate
-  draw(\_:in:) 

Instance Method

# draw(\_:in:)

Tells the delegate to implement the display process using the layer’s context.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
optional func draw(
    _ layer: CALayer,
    in ctx: CGContext
)
```

## Parameters 

`layer`  

The layer whose contents need to be drawn.

`ctx`  

The graphics context to use for drawing. The graphics context incorporates the appropriate scale factor for drawing to the target screen.

## Discussion

The draw(_:in:) method is called when the layer is marked for its content to be reloaded, typically with the setNeedsDisplay() method. It is not called if the delegate implements the display(_:) method. You can use the context to draw vectors, such as curves and lines, or images with the draw(_:in:byTiling:) method.

The following code shows how you can create a class named `LayerDelegate` that implements CALayerDelegate and sets it as a layer’s (named `sublayer`) delegate. When setNeedsDisplay() is called on `sublayer`, the delegate’s draw(_:in:) method draws an ellipse fitting the bounding box of the layer using the boundingBoxOfClipPath function.

```
let delegate = LayerDelegate()

lazy var sublayer: CALayer = {
    let layer = CALayer()

    layer.delegate = self.delegate

    return layer
}()

// sublayer.setNeedsDisplay()

class LayerDelegate: NSObject, CALayerDelegate {
    func draw(_ layer: CALayer, in ctx: CGContext) {
        ctx.addEllipse(in: ctx.boundingBoxOfClipPath)
        ctx.strokePath()
    }
}
```

Important

This method is not called if the delegate implements display(_:).

## See Also

### Providing the Layer’s Content

func display(CALayer)

Tells the delegate to implement the display process.

func layerWillDraw(CALayer)

Notifies the delegate of an imminent draw.

